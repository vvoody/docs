# Booting CoreOS Container Linux from an ISO

The latest Container Linux ISOs can be downloaded from the image storage site:

<div id="iso-images">
  <ul class="nav nav-tabs">
    <li class="active"><a href="#stable" data-toggle="tab">Stable Channel</a></li>
    <li><a href="#beta" data-toggle="tab">Beta Channel</a></li>
    <li><a href="#alpha" data-toggle="tab">Alpha Channel</a></li>
  </ul>
  <div class="tab-content coreos-docs-image-table">
    <div class="tab-pane" id="alpha">
      <div class="channel-info">
        <p>The Alpha channel closely tracks master and is released frequently. The newest versions of system libraries and utilities will be available for testing. The current version is Container Linux {{site.alpha-channel}}.</p>
      </div>
      <a href="https://alpha.release.core-os.net/amd64-usr/current/coreos_production_iso_image.iso" class="btn btn-primary">Download Alpha ISO</a>
      <a href="https://alpha.release.core-os.net/amd64-usr/current/" class="btn btn-default">Browse Storage Site</a>
      <br/><br/>
      <p>All of the files necessary to verify the image can be found on the storage site.</p>
    </div>
    <div class="tab-pane" id="beta">
      <div class="channel-info">
        <p>The Beta channel consists of promoted Alpha releases. The current version is Container Linux {{site.beta-channel}}.</p>
      </div>
      <a href="https://beta.release.core-os.net/amd64-usr/current/coreos_production_iso_image.iso" class="btn btn-primary">Download Beta ISO</a>
      <a href="https://beta.release.core-os.net/amd64-usr/current/" class="btn btn-default">Browse Storage Site</a>
      <br/><br/>
      <p>All of the files necessary to verify the image can be found on the storage site.</p>
    </div>
    <div class="tab-pane active" id="stable">
      <div class="channel-info">
        <p>The Stable channel should be used by production clusters. Versions of Container Linux are battle-tested within the Beta and Alpha channels before being promoted. The current version is Container Linux {{site.stable-channel}}.</p>
      </div>
      <a href="https://stable.release.core-os.net/amd64-usr/current/coreos_production_iso_image.iso" class="btn btn-primary">Download Stable ISO</a>
      <a href="https://stable.release.core-os.net/amd64-usr/current/" class="btn btn-default">Browse Storage Site</a>
      <br/><br/>
      <p>All of the files necessary to verify the image can be found on the storage site.</p>
    </div>
  </div>
</div>

## Known limitations

1. UEFI boot is not currently supported. Boot the system in BIOS compatibility mode.
2. There is no straightforward way to provide an [Ignition config][cl-configs].
3. A mininum of 2 GB of RAM is required to boot Container Linux via ISO.

## Install to disk

The most common use-case for this ISO is to install Container Linux to disk. You can [find those instructions here](installing-to-disk.md).

## No authentication on console

The ISO is configured to start a shell on the console without prompting for a password. This is convenient for installation and troubleshooting, but use caution.

[cl-configs]: provisioning.md
