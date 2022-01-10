<h1>Simple Docker Mini Project</h1>
<br>
<h2>Description</h2>
This is a simple docker project. Here we deploy multiple containers as listed below - 
<ol>
 <li><strong>XYZ Site</strong> - This is a static Website using NGINX</li>
 <li><strong>MYSQL Server</strong> - Deployed a MYSQL DBMS Server at the Port 3306</li>
 <li><strong>Phpmyadmin</strong> - This is the Web Frontend for managing the Deployed MYSQL Server</strong>
 <li>
<strong>Website Redirection Server</strong> - This is a Webserver whose purpose is to redirect the Client to either the Site [1] or the Site [3]
	<ul>
		<li>If the Client Request is in the format http://&lt;domain&gt;/ or http://&lt;domain&gt;/xyz then the Server redirects to XYZ Site</li>
		<li>If the Client Request is in the format http://&lt;domain&gt;/db then the Server redirects to the Phpmyadmin Site</li>
	</ul>
</li>
</ol>


