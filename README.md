<h1>Simple Docker Mini Project</h1>
<br>
<h2>Description</h2>

This is a simple docker project. Here we deploy multiple containers as listed below - 
<ol>
 <li><strong>XYZ Site</strong> - This is a static Website using NGINX</li>
 <li><strong>MYSQL Server</strong> - Deployed a MYSQL DBMS Server at the Port 3306</li>
 <li><strong>Phpmyadmin</strong> - This is the Web Frontend for managing the Deployed MYSQL Server</strong>
 <li>
<strong>Website Redirection Server</strong> - This is an NGINX Webserver whose purpose is to redirect the Client to either the Site [1] or the Site [3]
	<ul>
		<li>If the Client Request is in the format http://&lt;domain&gt;/ or http://&lt;domain&gt;/xyz then the Server redirects to XYZ Site</li>
		<li>If the Client Request is in the format http://&lt;domain&gt;/db then the Server redirects to the Phpmyadmin Site</li>
	</ul>
</li>
</ol>
<h2>Purpose</h2>

The Purpose of the project was to demonstrate that - 
<ol>
	<li>We can Deploy Multiple Services using docker</li>
	<li>Some of the Services (MYSQL and Phpmyadmin) can interact with each other using Internal Docker Networking</li>
	<li>Docker makes the work of deploying multiple services more resilient since each service is hosted in a seperate container, the environments are isolated from each other. This helps in ensuring that failure in a particular container does not disrupt the other services</li>
	<li>Deploying multiple containers does not lead to compatibility issues which can be faced in traditional deployments</li>
</ol>

<h2>Architecture</h2>

