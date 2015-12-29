# struts-convention
introduction to struts convention


#Dependency required

```
<dependency>
			<groupId>org.apache.struts</groupId>
			<artifactId>struts2-convention-plugin</artifactId>
			<version>{Version}</version>
</dependency>
```
Struts filter in web.xml
```
  <filter>
		<filter-name>struts2</filter-name>
		<filter-class>org.apache.struts2.dispatcher.ng.filter.StrutsPrepareAndExecuteFilter</filter-class>
	</filter>

	<filter-mapping>
		<filter-name>struts2</filter-name>
		<url-pattern>/*</url-pattern>
	</filter-mapping>
```	
Write all your action classes in **actions** package e.g. **com.example.actions**
### For "/" root path create Index.java class and  index.jsp view file
### For ```<anyname>``` use ```<Anyname>```.java class and ```<anyname>```.jsp view file
##### e.g. http://localhost:8080/webappName/main 
##### com.example.actions.Main.java and main.jsp
### For /```<urlPath>/<Page>``` use ```<Page>```.java class in ```<urlPath>``` package with view file under folder ```<urlPath>``` and name page.jsp
##### e.g. http://localhost:8080/webappName/list/display 
##### com.example.actions.list.Display.java and list/display.jsp
