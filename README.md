# EX01 Developing a Simple Webserver

# Date:19.09.2025
# AIM:
To develop a simple webserver to serve html pages and display the configuration details of laptop.

# DESIGN STEPS:
## Step 1:
HTML content creation.

## Step 2:
Design of webserver workflow.

## Step 3:
Implementation using Python code.

## Step 4:
Serving the HTML pages.

## Step 5:
Testing the webserver.

# PROGRAM:
"""
from http.server import HTTPServer,BaseHTTPRequestHandler
content = '''
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>TCP/IP Protocol Suite</title>
    <style>
      body{
        font-family: Arial, sans-serif;
        display: flex;
        justify-content: center;
        padding: 15px;
        border-radius: 10px;de())
print("This is my webserver")
server_address =('',8000)
httpd = HTTPServer(server_address,MyServer)
httpd.serve_forever()
    }
    .column {
        width: 260px;
        border: 2px solid #333;
        border-radius: 8px;
        overflow: hidden;
    }
    .column h2 {
        text-align: center;
        margin: 0;
        background: #2c3e70;
        color: white;
        padding: 8px;
        font-size: 18px;
    }
    .layer {
        border: 1px solid white;
        color: black;
        margin: 0;
        padding: 25px;
        text-align: center;
        font-weight: bold;
    }
    .internet { background: #1a1a1a; color: white; }
    .application { background: #4caf50; color: white; }
    .transport { background: #673ab7; color: white; }
    .network { background: #ff9800; color:white; }
     
    .protocol-section {
        text-align: center;
        padding: 10px;
    }
    .protocol-group{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 10px;
        margin: 8px 0;
    }
    .protocol {
        background: #0d47a1 ;
        color: white;
        padding: 6px 12px;
        border-radius: 4px;
        font-size: 14px;
        font-weight: bold;
    }
    .tcpudp {
        background: #4caf50 ;
        color: white;
        padding: 10px 20px;
        border-radius: 4px;
        font-weight: bold; 
    }
    .ip{
        background: #673ab7;
        color: white;
        padding: 10px 20px;
        border-radius: 4px;
        font-weight: bold;
    }
    .subprotocol {
        background: #ef6c00;
        color: white;
        padding: 10px;
        border-radius: 4px;
        font-size: 14px;
        font-weight: bold;
        flex: 1 1 40%;
        text-align: center;
    }
</style>
</head>
<body>
    <div class="container">
        <h2>TCP/IP Model</h2>
        <div class="layer internet">Internet
        layer</div>
    </div>
    <div class="layer application">Application layer</div>
    <div class="layer transport">Transport Layer</div>
    <div class="layer network">Network Interface Layer</div>

    <div class="row">
        <h2>TCP/IP Protocol Suite</h2>
        <div class="protocol-group">
            <div class="protocol">HTTP</div>
            <div class="protocol">FTP</div>
            <div class="protocol">TFTFP</div>
            <div class="protocol">DNS</div>
            <div class="protocol">DHCP</div>
            <div class="protocol">SMTP</div>
            <div class="protocol">Telnet</div>
        </div>
        <div class="protocol-group">
            <div class="protocol">TCP</div>
            <div class="protocol">UDP</div>
        </div>
        <div class="protocol-group">
            <div class="protocol">IP</div>
        </div>
        <div class="protocol-group">
            <div class="subprotocol">Ethernet</div>
            <div class="subprotocol">Token Ring</div>
            <div class="subprotocol">Frame Relay</div>
            <div class="subprotocol">ATM</div>
        </div>
    </div>

    
</body>
</html>
'''
        
  
class MyServer(BaseHTTPRequestHandler):
    def do_GET(self):
        print("Get request received...")
        self.send_response(200)
        self.send_header("content-type","text/html")
        self.end_headers()
        self.wfile.write(content.encode())
print("This is my webserver")
server_address =('',8000)
httpd = HTTPServer(server_address,MyServer)
httpd.serve_forever()
"""
# OUTPUT:
![alt text](<Screenshot 2025-09-19 202549.png>)
![alt text](<Screenshot 2025-09-19 202824.png>)


# RESULT:
The program for implementing simple webserver is executed successfully.
