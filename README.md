SrcMixins4J / Eclipse
=====================

Source code based mixins for Java / Eclipse Plugin

Installation
------------

1. Inside Eclipse click menu "Help / Install New Software..."
2. Press "Add" button to add the repository: http://www.fuin.org/p2-repository
3. Install "JaMoPP (Java Model Parser and Printer)"  
   [CAUTION: Installation together with "SrcMixins4J" in one step does currently not work] 
4. Restart Eclipse
5. Install "SrcMixins4J"
6. Restart Eclipse
7. Import [srcmixins4j-eclipse-example](https://github.com/fuinorg/SrcMixins4J/tree/master/examples/srcmixins4j-eclipse-example) from GitHub into your workspace
8. Ignore the build error and restart Eclipse  
   [This is a known bug - Will be solved soon]
9. Project / Clean "srcmixins4j-eclipse-example"
10. Open [AnotherClass](https://github.com/fuinorg/SrcMixins4J/blob/master/examples/srcmixins4j-eclipse-example/src/org/fuin/srcmixins4j/test/AnotherClass.java), 
add "implements NamedMixin&lt;String&gt;" and save your changes. If everything works, the mixin code is added.

**IMPORTANT**: Make sure that you always add a "srcMixins4JNature" to the Eclipse ".project" file if you want to use SrcMixins4J:
```xml
<projectDescription>
	...
	<natures>
		...
		<nature>org.fuin.srcmixins4.srcMixins4JNature</nature>
	</natures>
</projectDescription>
```
