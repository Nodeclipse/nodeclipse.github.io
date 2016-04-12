---
layout: nil
---

This is Eclipse update site. URL should be entered in Help -> Install New Software...

# Polyglot Maven with YAML IDE Pack (bleeding edge)

Break your build by experimenting with Polyglot Maven POC (aka Prove of Concept, aka alpha),
and loose your `pom.xml` file(s) completely unless it has been in version control, 
e.g. `git init`, `git add pom.xml`, 'git commit -m "pom save me"'.

After installing this pack (and Eclipse IDE restart), convert your `pom.xml` into nice shiny `pom.yaml`
and edit 50 lines inteads of 1000 using nice and steady [YEdit YAML Editor](https://github.com/oyse/yedit)
 by Øystein Torget, who is now 
[interested in making it standard within Eclipse IDE](https://github.com/oyse/yedit/issues/37).

Press <kbd>Ctrl+Alt+T</kbd> or <kbd>Ctrl+Alt+D</kbd> to launch local terminal, and launch translation:

	mvn io.takari.polyglot:polyglot-translate-plugin:translate -Dinput=pom.xml -Doutput=pom.yaml
	
Convert an existing Maven (m2e) project into Polyglot Maven via right-click on a project and 
`Configure > Convert to Maven Polyglot...`

Edit `pom.xml` and see it instantly converted into `pom.xml` (so you can still enjoy extra informative tabs in m2e POM Editor)
and changes applied to the project. 

Never read docs, software can guess your intentions and act in your best interests always.

## Links

- https://github.com/takari/polyglot-maven
- https://github.com/takari/polyglot-maven-examples
- https://github.com/jbosstools/m2e-polyglot-poc

{% include navigation-links.html %}