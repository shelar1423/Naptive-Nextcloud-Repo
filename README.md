
&nbsp;

<p align="center">
  <a href="https://nextcloud.com/#gh-dark-mode-only" target="_blank">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/Nextcloud_Logo.svg/1200px-Nextcloud_Logo.svg.png" alt="nextcloud" width="440px">
  </a>
</p>
&nbsp;
<p align="center">
    <a href="https://nextcloud.com/">nextcloud.com</a> •
    <a href="https://docs.nextcloud.com/server/26/admin_manual/installation/index.html">Docs</a> •
    <a href="https://github.com/nextcloud">Github</a> •
    <a href="https://twitter.com/Nextclouders">Twitter</a>
    <br /><br />
<hr><hr>

![image](https://user-images.githubusercontent.com/82649533/232209599-64649ab6-ff0b-4715-a282-121e3d75aae1.png)

&nbsp;

<ul>
<li><h1>What is Nextcloud?</h1></li>
</ul>
A safe home for all your data. Access & share your files, calendars, contacts, mail & more from any device, on your terms.

Nextcloud.com

<a href="https://nextcloud.com/#gh-dark-mode-only" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/Nextcloud_Logo.svg/1200px-Nextcloud_Logo.svg.png" alt="Nextcloud(Pro)" width="165px" /></a>

This Docker micro-service image is developed and maintained by the Nextcloud community. Nextcloud GmbH does not offer support for this Docker image. When you are looking to get professional support, you can become an enterprise customer or use AIO.
&nbsp


<ul>
<li><h1>How to use Nextcloud</h1></li>
</ul>
- First, make sure you have a web server, PHP, and a database management system installed.
- Download Next from their website and extract it to a folder on your web server.
- Create a new database and user for Nextcloud.
- Open your web browser, go to the Nextcloud URL, and follow the installation instructions.
- To upload files, log in to Nextcloud and click "Upload" to select and upload files.
- To share files, click "Share" next to the file, enter the email of the person you want to share with, and click "Send".
- To synchronize files, download and install the Nextcloud desktop client, log in, select the files to sync, and click "Sync".
<ul>
<li><h1>How to Deploy Nextcloud on NAPPTIVE PLAYGROUND</h1></li>
</ul>

Before Deploying the application on NAPPTIVE first we need to create an OAM file(Open Application model) for doing this we need to create a YAML file in which we can add the component and properties required to migrate the application in OAM.

![28254b42-190e-4a12-876f-1da2e9095c70](https://user-images.githubusercontent.com/82649533/232207883-115659aa-c311-45ac-a3c3-be6d7a4fa33c.jpg)


A Component represents a single microservice from the Application. To define it, select the type of component that adapts best to the use case, and define its properties. here I have choose webservice(Describes long-running, scalable, containerized services that have a stable network endpoint to receive external network traffic from customers) 

<ul>
<li><h1>Traits</h1></li>
</ul>
A Trait represents an extension for an application component. This facilitates reusing components in different situations, and simplifies their packaging as the developer does not need to add any extra information for its deployment. For example, exposing an application component to the public Internet can be easily done by attaching an ingress trait. The trait offers the same abstraction as the component and will create the underlying ingress attending to the installed controller and cloud provider. In this way, the developer can publish the component with its parameters, and when creating the application, the ingress can be easily added. Other examples of traits include mounting volumes, adding labels, exporting logs, exploring monitoring information, etc.
In my case I used napptive-ingress(Expose a component to the outside with a K8s ingress)

![33ecc005-c495-4fcb-b061-ce411a235ce9](https://user-images.githubusercontent.com/82649533/232207958-297927c3-acd4-43e6-a628-67a095f2331d.jpg)


After you've completed all of this, upload the yaml file to the NAPPTIVE platform and click the Deploy button. 

![image](https://user-images.githubusercontent.com/82649533/232208014-60010b61-427f-4c7d-ab17-7d0249748b9d.png)

Finally, you can see on the screen that your application is running.

![image](https://user-images.githubusercontent.com/82649533/232208197-1dba84bc-b3ee-4154-a956-df9495a1cd26.png)

<ul>
<li><h1>Acessing after deployment</h1></li>
</ul>
After deployment click on the endpoint link you will see this interface to access Nextcloud

![image](https://user-images.githubusercontent.com/82649533/232208417-4054abc0-78cd-42ee-ba30-588a70fc8028.png)


