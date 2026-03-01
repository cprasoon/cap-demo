# Load balancing with Nginx

## 1-Load balancer & 3Nginx instances
Very easy setup
1) Move to configuration folder
2) Docker compose up
3) Manual-verification
    1) Goto localhost, Check with page got served.  
    It will cycle between Red,Blue and Green NGINX pages
4) Jmeter test run
    1) move to test folder (ensure jmeter is on you path)  
    jmeter.bat -n -t httpRequestToNginx.jmx -l ..\build\out.jtl -e -o ..\build\result1