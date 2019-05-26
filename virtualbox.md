## VM 복사하기
  1. export
     ```
     VBoxManage import vui-voiceable02/vui-voiceable02.ova --vsys 0 --vmname vui-voiceable02
     ```
  2. import :
     ```
     VBoxManage export vui-voiceable01 --output vui-voiceable02/vui-voiceable02.ova
     ```
  * [참고](https://www.techrepublic.com/article/how-to-clone-virtualbox-virtual-machines-from-the-command-line/)

## 마우스 포인터 캡처 해제

```
VBoxManage setextradata "VM name" GUI/MouseCapturePolicy Disabled
```

 [참고](https://superuser.com/questions/214414/how-to-permanently-disable-mouse-integration-in-virtualbox)
  
