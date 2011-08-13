NEXT
====

NEXT is a Java GWT UI framework for developing Native Looking HTML5 Mobile applications for SmartPhones and Tablets.

More information:
-----------------
   http://nextinterfaces.com/


DEMO (WebKit only):
-------------------
   http://nextinterfaces.com/DEMO
 

Documentation:
--------------
   http://nextinterfaces.com/START


Dependencies:
-------------
   Java5+
   GWT (Google Web Kit) 2.2+


Supported Phones & Tablets:
---------------------------
   iOS, Android, BlackBerry OS6+, BlackBerry PlayBook, Samsung Bada, Palm webOS
   
	
Installation:
-------------
* Download NEXT zip file from http://nextinterfaces.com/DOWNLOAD
* Add the attached /hello-next project to Eclipse. Eclipse should automatically discover it as a GWT project.
* From Eclipse /Run /Run As Web Application.
* Alternatively, you can also copy next.jar (hello-next/war/WEB-INF/) file to your GWT project and add it to your classpath.


Hello World in 30 seconds:
--------------------------
1. Create a new GWT project
2. Add next.jar to project classpath
3. Create class HelloWorldController

      class HelloWorldController extends XTableController {
        public HelloWorldController() {
          setTitle("Hello World");
          TableData tableDS = new TableData();
          tableDS.add("Hello", "World");
          initDataSource(tableDS);
        }
      }

      
4. In your EntryPoint class type

      public void onModuleLoad() {
        XTabBarController tabBarController = new XTabBarController();
        tabBarController.addControllers(new XTabController(new HelloWorldController()));
      }

      
   5. Eclipse /Run /Run as Web Application
      Resulting in http://goo.gl/fFQXY

See the attached /hello-next project or /next-demo https://github.com/nextinterfaces/next-demo for more information.
 