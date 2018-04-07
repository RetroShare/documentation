Start by getting the RetroShare code from our [git repository](https://github.com/RetroShare/RetroShare).

Then make sure to read the [README.md](https://github.com/RetroShare/RetroShare/blob/master/README.md) file in the main RetroShare source directory.

In the [README.md](https://github.com/RetroShare/RetroShare/blob/master/README.md) you can find information about building that is the next step to do.


## Coding Style

Although initial coding of RetroShare did not followed any particular coding 
style, we would like to start using a strict coding style. It can happen to you 
that while you read the code you start hating who written it because she didn't
followed the code convention, in that case please avoid to drop a
non-constructive rant in public or doing something worse and try to chill out
before expressing your opinion remembering that RetroShare code has been 
written by volunteers and that they are nice people despite the fact you are
suffering reading some part of the code.

Officially RetroShare is using the [Allman indent style](http://en.wikipedia.org/wiki/Indent_style#Allman_style) 
using tabulator as indent char +\t+ *not* the white space which instead is used 
for alignment and as separator. This choice that have many advantage 
is motivated not just by tastes but in respect of every developer, if 
you use spaces (for example 8 spaces per indent) for indentation all 
developers are forced to see same number of spaces for each indent thus 
causing developers with little screen hating you, instead if you use 
tabulators each developer can configure his editor to display them 
the size they feel more comfortable. Please keep your lines under 80 
columns unless it doesn't cause the code to 
look ugly to facilitate code editing and diff also on small screens.

If you use [Qt Creator](https://en.wikipedia.org/wiki/Qt_Creator) you can
download and import
[RetroShare Qt Creator C++ coding style](Qt_Creator_RetroShare_Cxx_coding_style.xml)
and
[RetroShare Qt Creator QML coding style](Qt_Creator_RetroShare_QML_coding_style.xml)
and set it as coding style for RetroShare project, pay attention that at moment
Qt Creator is not capable of enforcing Allman indent style on QML files so you
will have to do it by yourself.


## Bad Practices

### Overlook compiler warnings

Compiler warning are not to annoy the developers but to help them to avoid dangerous code, when a compiler warn about something on your code you must take in account, and make sure your compiler warnings count is *0* before pushing to the repository. The fact that the compiler warning on the code hosted on the repository is 0 is very important because if your modification introduce a warning (aka potential error) you will notice it easily, instead if the code on the repository have already compilers warnings it is unlikely that you will pay attention to the ones you just introduced in your last modification.


### Code Copy/Paste

Avoid copy pasting code around as this is a common source of bugs, instead
abstract the code when possible.


### Unuseful code 

Avoid not useful statements like ending a void method with return.

```cpp
virtual ~p3PeerMgr() { return; }
```

The return there just make the code bloated, instead use this semantically
equivalent but more elegant form.

```cpp
virtual ~p3PeerMgr() {}
```

### Overload Hiding

An enough common but subtle error is when you think you have overloaded a
parent class method but you really haven't.

```cpp

class PQInterface
{
public:
	virtual int notifyEvent(NetInterface * /*ni*/, int /*event*/,
	    const sockaddr_storage & /*remote_peer_address*/)
	{ return 0; }
};

class pqiloopback: public PQInterface
{
	virtual int notifyEvent(NetInterface /*ni*/, int /*event*/,
	    const sockaddr_storage /*remote_peer_address*/)
	{ return doSomethingElse(); }
};

```

Pay attention to the type of parameters as the compiler do, or you will end up
having a difficult to tackle down unexpected behaviour.

### Unused named parameters casting

When implementing a method that does have unused parameters for a good reason,
like to match the type of an interface, you should avoid to use unuseful cast
to avoid compiler warning:

```cpp

class pqiloopback: public PQInterface
{
	virtual int notifyEvent(NetInterface *ni, int event,
	    const sockaddr_storage & remote_peer_address)
	{
		(void) ni; (void) event; (void) remote_peer_address;
		return 1;
	}
};

```

instead comment the parameter name:

```cpp

class pqiloopback: public PQInterface
{
	virtual int notifyEvent(NetInterface * /*ni*/, int /*event*/,
	    const sockaddr_storage & /*remote_peer_address*/)
	{ return 1; }
};

```


### Avoid possible conflicting identifiers

The problems we experienced compiling for Windows due to the usage of apparently
innocent identifiers such as `lst1`, `lst2`, `grp1`, `grp2` suggest we should be
expecially carefull in chosing identifiers names, so avoid to use names that may
easly create conficts with system and library macros such as `win32`, `unix`
etc.

In this web-page you can find a list of names not usable on Windows
https://doc.pcsoft.fr/en-US/?6510001 .
