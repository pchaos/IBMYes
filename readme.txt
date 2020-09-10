wget --no-check-certificate -O install.sh https://raw.githubusercontent.com/pchaos/IBMYes/master/install2.sh && chmod +x install.sh  && ./install.sh

cf套cdn脚本

addEventListener(
"fetch",event => {
let url=new URL(event.request.url);
url.hostname="ibmyes.us-south.cf.appdomain.cloud";
let request=new Request(url,event.request);
event. respondWith(
fetch(request)
)
}
)


cf测速：
104.17.154.107
104.18.250.14

