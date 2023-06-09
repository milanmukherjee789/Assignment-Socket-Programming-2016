# Simple chat application using Mulithreaded Socket programming in C++
<h2>Objective : </h2>
<p>
	In this project there will be one server and multiple clients. Among those clients any two clients can chat with each other. Server will have a sqlite database into which all informations corresponfing those clients will be stored.
</p>
<h2> Setup the environment: </h2>
<p> For socket programming we need some libraries and most of the linux operating system will have those headers and their binary pre-installed in the system. For this particular project we need sqlite3 headers and the binary. If sqlite3 binary and the header is not installed then we need to install them. The procedure is described as below: 
<ul>
	<li> Download the tar file from the link Given : <a href="http://www.sqlite.org/2017/sqlite-autoconf-3170000.tar.gz">sqlite-amalgamation-3170000.zip</a></li>
	<li>
		After downloading, install the library with the sqlite3 binary :
		<ol>
			<li>cd ~/Downloads</li>
			<li> tar xvfz sqlite-autoconf-3170000.tar.gz</li>
			<li>cd sqlite-autoconf-3170000</li>
			<li>./configure --prefix=/usr/local</li>
			<li>sudo make</li>
			<li>sudo make install</li>
		</ol>
	</li>
</ul>
</p>
<h2> How to Run the Application : </h2>
<p>
	<h4> To run the Server : </h4>
	<ol>
		<li> <strong> Create the database -> </strong><span style="color: blue">./DB_Create</span></li>
		<li><strong> Run the server -> </strong><span style="color: blue">./run.sh</span></li>
	</ol>
	<h4> To run the client : </h4>
	<ul><li><span style="color: blue">./client1 "Server IP address" "PORT NO" </span></li></ul>
	<p> Run the client from different terminals to create multiple clients or run the client in different physical machines.</p>
</p>