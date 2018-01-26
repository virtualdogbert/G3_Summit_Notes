Groovy by the Numbers

    30+ new contributors in the last 12 months
    4+ million downloads per month (23m 2016, 40m 2017)
    Groovy 2.4, 2.5, 2.6, 3.0 release chains in progress:
        - 3.0.0-alpha-1: 2017-11-29
        - 2.4.13: 2017-11-23
        - 2.6.0-alpha-2: 2017-11-15
        - 2.5.0-beta-2: 2017-10-02
        - 2.6.0-alpha-1: 2017-09-06
        - 2.4.12: 2017-06-24
        - 2.5.0-beta-1: 2017-06-06
        - 2.4.11: 2017-04-28
        - 2.5.0-alpha-1: 2017-04-02
        - 2.4.10: 2017-03-18
        - 2.4.9: 2017-02-27
        - 2.4.8: 2017-01-14

Groovy 2.5
* Beta-2 out now, RCs coming soon, GA first half of 2018
* Macros, AST transformation improvements, various misc features
* JDK 7 minimum, runs on JDK 9/10 with warnings

Groovy 2.6/3.0
* Alphas out now, RCs by end 2018
* Parrot parser, various misc features
* JDK 8 minimum (3.0), address most JDK 9/10 issues
* 2.6 is a back port of 3 for JDK 7

Groovy Podcast Episodes 50 and 50.5:
* https://www.youtube.com/watch?v=SZHeKHycKWk
* https://www.youtube.com/watch?v=3NLPVfYLdGc

G3 Summit Blog posts:
* https://giri-tech.blogspot.com/2017/12/g3-summit-2017-great-experience.html
* https://erichelgeson.github.io/blog/2017/12/02/g3summit/


AST

    In Transforms AstNode[] always has two values the node being transformed and the annotation node.
    You see some param checking is most AST transforms this can be discarded, was from when Groovy was less stable.
    Uses for Source Unit
        Fixing variable scope
        Adding compile errors
        Get classes for global AST
    GeneralUtils helps simplify some common AST patterns(callX, stmt, etc from utils but will probably be replace with Macro methods)
    VariableScopeVisitor is run early in the compliation process, but can be useful for cleaning up when you add code that needs to have it's scope set. Manually messing with variable scope can get you into trouble.
    Macros are good for statements and expressions can just write groovy, has placeholders to inject variables from outside.
        http://docs.groovy-lang.org/docs/groovy-2.5.0-beta-2/html/documentation/#_macros


    Ask about the idea of compiling to webassembly using groo script as a jumping off point.
    No one really even knew about it, started getting a lecture about how trying to replace JS was not usually a good idea. When the host corrected them telling them about how it was a byte code not a JS replacement
    they shrugged I think it was good just to put the idea on there radar.

    Grails questions
        Ask about the utility of Data services.
        saw them seem like they could be interesting, there utility will depend on the use case.

    Ask about RX Gorm, support, error handling, file handling.
    Not a lot of people interested, ask again

    It's very easy to make a Grails jar exacutable and it knows how to be a service:
        comment out war plugin

        springBoot{
             executable = true
            ....
        }

        ln -s /ect/init.d/myapp exacuteable-jar

Gradle
* https://docs.google.com/document/d/1LL_WqCNp1lFmX_4pKW04Q2S0ZyP5QfZu8ZwoHEnejbE/edit
* http://www.kousenit.com/gradle/
* https://plugins.gradle.org/search?term=static
* https://discuss.gradle.org/


Other Conferences:
* http://gr8conf.us/
* http://gr8conf.eu/#/
* http://2018.greachconf.com/

If you would like to get a Groovy/Grails tshirt like mine use the link below. I get some type of royalty for it that I've decided that I will just donate to a charity. I'm choosing Autism Speeks, just because I once saw Jeff Scott Brown tweet about it;

https://www.customizedgirl.com/s/groovygrailsshwag

