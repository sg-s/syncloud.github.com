---
layout: device
title: Cubietruck

boardname: Cubietruck
releaseversion: v0.6
imagefile: syncloud-cubietruck-v0.6.img
---

<div class="row">

    <div class="col-6 col-md-6 col-sm-6 col-lg-6">
        <h3><span class="label label-success">1. Get Hardware</span></h3>
        <img class="center-block img-responsive" src="images/board-cubietruck.png" style="padding: 13px"/>

        <p>Buy <a href="http://cubieboard.org/buy">Cubietruck A20</a> single-board computer and SATA hard drive.
        </p>
    </div>

    <div class="col-6 col-md-6 col-sm-6 col-lg-6">
        <h3><span class="label label-success">2. Get Software</span></h3>

        <img class="center-block img-responsive" src="images/software-debian.png"/>

        <p>Download syncloud image for <a onClick="_gaq.push(['_trackEvent', 'Images', 'Download', '{{page.boardname}} {{page.releaseversion}}']);" href="https://github.com/syncloud/owncloud-setup/releases/download/{{page.releaseversion}}/{{page.imagefile}}.xz">{{page.boardname}}</a>.
        </p>
    </div>

</div>

<div class="row">

    <div class="col-6 col-md-6 col-sm-6 col-lg-6">
        <h3><span class="label label-success">3. Install Software</span></h3>
        <br>
        <p>Create microSD card (2GB or more):</p>
        <div>
            <p><span class="badge">1</span><span style="padding-left: 10pt">Uncompress image file (Linux/Mac):</span></p>
            <p><span style="padding-left: 25pt"></span><code>unxz {{page.imagefile}}.xz</code></p>
            <p><span style="padding-left: 25pt">Or use <a onClick="_gaq.push(['_trackEvent', '7Zip', 'Download', '{{page.boardname}} {{page.releaseversion}}']);" href="http://www.7-zip.org">7-zip</a> on Windows</p>

            <p><span class="badge">2</span><span style="padding-left: 10pt">Write image to SD card (Linux/Mac):</span></p>
            <p><span style="padding-left: 25pt"></span><code>sudo dd if=./{{page.imagefile}} of=/dev/mmcblk0</code></p>
            <p><span style="padding-left: 25pt"></span>Or use <a onClick="_gaq.push(['_trackEvent', 'win32diskimager', 'Download', '{{page.boardname}} {{page.releaseversion}}']);" href="http://sourceforge.net/projects/win32diskimager">Win32 Disk Imager</a> on Windows</p>

            <p><span class="badge">3</span><span style="padding-left: 10pt">Insert SD card into device</span></p>
            <p><span class="badge">4</span><span style="padding-left: 10pt">Power on</span></p>
        </div>
        <p>Syncloud image is based on <a onClick="_gaq.push(['_trackEvent', 'Cubian', 'Download', '{{page.boardname}} {{page.releaseversion}}']);" href="http://www.cubian.org/downloads/">Cubian</a></p>
    </div>

    <div class="col-6 col-md-6 col-sm-6 col-lg-6">
        <h3><span class="label label-success">4. Connect Everything</span></h3>
        <br>
        <p>Connect hard disk drive to the device. You can use SATA or USB connector. Don't forget to create ext4 partition on the drive.<br/>Connect your device to your home router. Use one of the available LAN ports.<br/>Turn the device on.
        </p>
        <img class="center-block img-responsive" src="images/schema-cubietruck-logo.png" style="max-width: 80%; margin: 0 auto"/>
    </div>

</div>
