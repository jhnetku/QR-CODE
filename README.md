# qrlogin - HMS
## QR Code scanner for login hotspot MikroTik

### Cara pakai

1. Tambahkan code button di login.html
```
<button onclick="window.location='https://github.com/jhnetku/QR-CODE/?hotspot=Nama Hotspot Anda';">QR Login</button>
```
2. Tambahkan script berikut di MikroTik via terminal.
```
/ip hotspot walled-garden ip
add action=accept comment="JHNET QR Code Scanner" disabled=no dst-host=hotspotms.github.io
```
