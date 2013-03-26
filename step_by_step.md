Presentation for [ConFESS](https://2013.con-fess.com/)
--------------------------
This github repository hold all the slides material required to follow the step by step tutoreial to build a clone of Fousquare in a few minutes. The application we're going to build will be name ThreeCircle ;-)

## Step1: Scaffolding
###create-app
grails create-app ThreeCircles
###BuildConfig.groovy
add
  grails.plugin.location."html5-mobile-scaffolding" = "../html5-mobile-scaffolding"
  grails.plugin.location."phonegapbuild" = "../phonegapbuild"

in plugins
'''java
    plugins {
        runtime ":hibernate:$grailsVersion"
        runtime ":jquery:1.9.1"
        runtime ":resources:1.1.6"
        build ":tomcat:$grailsVersion"
        runtime ":database-migration:1.1"
        compile ':cache:1.0.0'
        // http://support.cloudfoundry.com/entries/21014643-Grails-Spring-Security-deployment-problem
        // to fix cf/springsecurity issue
        compile ":webxml:1.4.1"
    }
'''


### Speakers
- [Corinne Krych](http://corinnekrych.github.com/)
- [Fabrice Matrat](http://fabricematrat.github.com/)

We're presenting you the work done by [3musket33rs](http://3musket33rs.github.com/) team.

### Step by Step tutorial
Off course these slides should be used with the tutorial [ThreeCircleConFESS]()

### Thanks to
[impress.js](http://bartaz.github.com/impress.js/) for doing so cool HTML5 presentations.
