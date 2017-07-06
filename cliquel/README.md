# Cliquel

----
## Description

> What a fat binary!
> 
> Note: Best effort is done so that only the canonicalized form is possibly accepted by the program; however, if you are sure the answer you deduced is correct but is not recognized by the platform, please do not hesitate to contact the organizers so that you (or your team) may get a chance to earn the points.
> 
> - This challenge exploits a property of Java ClassLoader for its obfuscation technology.
> - If you know how the challenge and its algorithm work, it would take virtually no time to solve it and considering all constraints there are very few possible cases for input.
> - This is NOT a heavy cryptography problem; inverse operation is unnecessary.
> 
> EDIT (09:37 UTC): Corrected an typo (its algorithm works -> its algorithm work)
> 
> There indeed are some classic nasty obfuscation tricks in both Java and native, but nevermind - the bottom line of all these stuffs are: what if everything was a class *cough* a classloader?
> 
> Namespaces of classes aren't global; rather, they are more like... *cliques*. Try to focus more on the native part. When you have both the answer string (hint: it's an encoded directed graph) and an appropriate standard J2SE 8 VM (java) program in your PATH, the flag will be just there - right in front of you - through the standard output stream.
> 
> Additional Hints (22:10 UTC)
> 
> Let me clarify: **All 22 classes (excluding the entry point) get loaded and used in the VM process should the program be given the correct answer.** As such, all classes may (either directly or indirectly) communicate with each other in the process of validating the input. However, due to duplicate class names some references may be ambiguous when they are resolved, and that's when the directed graph comes to play. Just remember: What You See Is Not What You Get.
> 
> [Download link](clique)

----
## Write-up

[View Image](writeup.svg)
