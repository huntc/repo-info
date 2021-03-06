<!-- THIS FILE IS GENERATED VIA './update-tag-details.sh' -->

# Tags of `ros`

-	[`ros:indigo-ros-core`](#rosindigo-ros-core)
-	[`ros:indigo-ros-base`](#rosindigo-ros-base)
-	[`ros:indigo`](#rosindigo)
-	[`ros:indigo-robot`](#rosindigo-robot)
-	[`ros:indigo-perception`](#rosindigo-perception)
-	[`ros:jade-ros-core`](#rosjade-ros-core)
-	[`ros:jade-ros-base`](#rosjade-ros-base)
-	[`ros:jade`](#rosjade)
-	[`ros:jade-robot`](#rosjade-robot)
-	[`ros:jade-perception`](#rosjade-perception)
-	[`ros:kinetic-ros-core`](#roskinetic-ros-core)
-	[`ros:kinetic-ros-base`](#roskinetic-ros-base)
-	[`ros:kinetic`](#roskinetic)
-	[`ros:latest`](#roslatest)
-	[`ros:kinetic-robot`](#roskinetic-robot)
-	[`ros:kinetic-perception`](#roskinetic-perception)

## `ros:indigo-ros-core`

```console
$ docker pull ros@sha256:9a0dac04bec4f0929bbe5e70c929956b2e38bf019a8115e717452ad002d7b6f5
```

-	Platforms:
	-	linux; amd64

### `ros:indigo-ros-core` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.6 MB (249619519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a544b337b5b26b09154fc74c387374bd1a4bab86a9b45fb6188ac8b88401a78f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 18 Jul 2016 17:34:50 GMT
ADD file:dc3b1b2c44af75026bc24b3f3a5bd5f45b9ca7ed395b91dfacd1b47fe0545fb5 in /
# Mon, 18 Jul 2016 17:34:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 18 Jul 2016 17:34:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 17:34:57 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Mon, 18 Jul 2016 17:34:58 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2016 19:05:53 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 19:05:56 GMT
RUN locale-gen en_US.UTF-8
# Mon, 18 Jul 2016 19:05:56 GMT
ENV LANG=en_US.UTF-8
# Mon, 18 Jul 2016 19:06:15 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Mon, 18 Jul 2016 19:06:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Mon, 18 Jul 2016 19:07:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:08:05 GMT
RUN rosdep init     && rosdep update
# Mon, 18 Jul 2016 19:08:06 GMT
ENV ROS_DISTRO=indigo
# Mon, 18 Jul 2016 19:10:38 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:10:40 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Mon, 18 Jul 2016 19:10:40 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Mon, 18 Jul 2016 19:10:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:96c6a1f3c3b0183063a9dad891fe6d8ec466c2fdf9571a0c19b3319ea8a58871`  
		Last Modified: Mon, 18 Jul 2016 17:36:54 GMT  
		Size: 65.7 MB (65699069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4767a2d70a73a271b76a76e4d5edf1426c49ccc24dc7df06ebccd880f01bbeab`  
		Last Modified: Mon, 18 Jul 2016 17:36:35 GMT  
		Size: 92.3 KB (92340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422639bc8a94f4f9ece99c13140bd78b9f25eb62492dd0402ffa4ec58b0d6d9b`  
		Last Modified: Mon, 18 Jul 2016 17:36:35 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a797489a324abb3d09826e5f5a529034aecdc962d54ca4dd642f9548c455295f`  
		Last Modified: Mon, 18 Jul 2016 17:36:35 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6675829cf13b49fb5d7afa4153cc834f0739bc7d25cacd7915bd58e9935da53`  
		Last Modified: Mon, 18 Jul 2016 19:10:54 GMT  
		Size: 329.2 KB (329185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffd474e471fc5604c08bd8925c1e19f391dba9c684ac1e65f4a0141c771b50d`  
		Last Modified: Mon, 18 Jul 2016 19:10:52 GMT  
		Size: 13.1 KB (13071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5645edeaaeed66f0df1c6bd4da8bbb5dd910a67c5323215a36aa8b9468ee9e`  
		Last Modified: Mon, 18 Jul 2016 19:10:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a82b6288ded8b62f1cd6625b1fee4ec208d2cf2f9e79a3ea599359b0c3bbc6`  
		Last Modified: Mon, 18 Jul 2016 19:11:04 GMT  
		Size: 32.9 MB (32870505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ea19c111a704f52c77df988862b9570734510cc71fb2981a640d5f9ecd8d24`  
		Last Modified: Mon, 18 Jul 2016 19:10:50 GMT  
		Size: 630.2 KB (630200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535cc521df40f09786be60d3a19726f4f2cc1e4a19e11d15f738e90d5aaf5611`  
		Last Modified: Mon, 18 Jul 2016 19:11:35 GMT  
		Size: 150.0 MB (149983681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8f8fe463f9e71c250ff9bb6065c0e565aee495201ab67a602bbdd26fbf43ad`  
		Last Modified: Mon, 18 Jul 2016 19:10:49 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-ros-base`

```console
$ docker pull ros@sha256:f93e3452dbf1b633b27517e142107965e47c7aab735f6e3b4d574d8d5e8d03d2
```

-	Platforms:
	-	linux; amd64

### `ros:indigo-ros-base` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.1 MB (253061114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403da81a44f824afd43f6216c73988047d467ac746d45076a06f0645802b3866`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:05:58 GMT
ENV ROS_DISTRO=indigo
# Fri, 24 Jun 2016 20:08:30 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:08:31 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:08:32 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:08:32 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:22:13 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:23:14 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb5969fba4a58ea911c5ec7a2926252c99415c77e58d963818232853aa6256`  
		Last Modified: Fri, 24 Jun 2016 20:09:24 GMT  
		Size: 150.0 MB (149983301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545b74da1b4d37ddb95f375586fb25f9c55739e75cd64febb0ae5db8cff905c8`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad2a859dd554ad916f7475a490727e14c8b7c7514b8a0b4c25513cfb65eb999`  
		Last Modified: Wed, 29 Jun 2016 19:23:23 GMT  
		Size: 3.4 MB (3448456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo`

```console
$ docker pull ros@sha256:f93e3452dbf1b633b27517e142107965e47c7aab735f6e3b4d574d8d5e8d03d2
```

-	Platforms:
	-	linux; amd64

### `ros:indigo` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.1 MB (253061114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403da81a44f824afd43f6216c73988047d467ac746d45076a06f0645802b3866`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:05:58 GMT
ENV ROS_DISTRO=indigo
# Fri, 24 Jun 2016 20:08:30 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:08:31 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:08:32 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:08:32 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:22:13 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:23:14 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb5969fba4a58ea911c5ec7a2926252c99415c77e58d963818232853aa6256`  
		Last Modified: Fri, 24 Jun 2016 20:09:24 GMT  
		Size: 150.0 MB (149983301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545b74da1b4d37ddb95f375586fb25f9c55739e75cd64febb0ae5db8cff905c8`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad2a859dd554ad916f7475a490727e14c8b7c7514b8a0b4c25513cfb65eb999`  
		Last Modified: Wed, 29 Jun 2016 19:23:23 GMT  
		Size: 3.4 MB (3448456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-robot`

```console
$ docker pull ros@sha256:7538966af6865a09ef6f58e064043bd82982cff3770b68394351316ccad506a6
```

-	Platforms:
	-	linux; amd64

### `ros:indigo-robot` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321255937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16cbed6fae6adab97c48dd12f948c66dcc73ce102f73d464c456f2461b54092e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:05:58 GMT
ENV ROS_DISTRO=indigo
# Fri, 24 Jun 2016 20:08:30 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:08:31 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:08:32 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:08:32 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:22:13 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:23:14 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:13:31 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:31:28 GMT
RUN apt-get update && apt-get install -y     ros-indigo-robot=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb5969fba4a58ea911c5ec7a2926252c99415c77e58d963818232853aa6256`  
		Last Modified: Fri, 24 Jun 2016 20:09:24 GMT  
		Size: 150.0 MB (149983301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545b74da1b4d37ddb95f375586fb25f9c55739e75cd64febb0ae5db8cff905c8`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad2a859dd554ad916f7475a490727e14c8b7c7514b8a0b4c25513cfb65eb999`  
		Last Modified: Wed, 29 Jun 2016 19:23:23 GMT  
		Size: 3.4 MB (3448456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8208a82d6705b8987c7e74645658f9150c787abd29ad1c82dcc2077cc207246`  
		Last Modified: Fri, 08 Jul 2016 19:32:14 GMT  
		Size: 68.2 MB (68194823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:indigo-perception`

```console
$ docker pull ros@sha256:43bd94d426acdc8a446b488883c5120919fb3ba319366835f3eb4a8a15fdf1f7
```

-	Platforms:
	-	linux; amd64

### `ros:indigo-perception` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **521.3 MB (521332502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4c65f60a1f7957e32da0835cce007f292e5e70e1c5e71b0f45b91696029e5bf`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:05:58 GMT
ENV ROS_DISTRO=indigo
# Fri, 24 Jun 2016 20:08:30 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-core=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:08:31 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:08:32 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:08:32 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:22:13 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:23:14 GMT
RUN apt-get update && apt-get install -y     ros-indigo-ros-base=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:13:31 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:19:11 GMT
RUN apt-get update && apt-get install -y     ros-indigo-perception=1.1.4-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aeb5969fba4a58ea911c5ec7a2926252c99415c77e58d963818232853aa6256`  
		Last Modified: Fri, 24 Jun 2016 20:09:24 GMT  
		Size: 150.0 MB (149983301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545b74da1b4d37ddb95f375586fb25f9c55739e75cd64febb0ae5db8cff905c8`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad2a859dd554ad916f7475a490727e14c8b7c7514b8a0b4c25513cfb65eb999`  
		Last Modified: Wed, 29 Jun 2016 19:23:23 GMT  
		Size: 3.4 MB (3448456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cbe2d4b9ded234692bf4712fad7fc93f1d06acfc80acdcd6ee619e4e27f7d2`  
		Last Modified: Fri, 08 Jul 2016 19:21:16 GMT  
		Size: 268.3 MB (268271388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:jade-ros-core`

```console
$ docker pull ros@sha256:31ae15c7e7537a3ae75901a3ccb8a8682db0686dbcbb60095d1d39a48128a379
```

-	Platforms:
	-	linux; amd64

### `ros:jade-ros-core` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249680600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:826c72bfaee55e4086feb03bb79e6701ab39eb7095443a0d1a015a2ecb11834d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 18 Jul 2016 17:34:50 GMT
ADD file:dc3b1b2c44af75026bc24b3f3a5bd5f45b9ca7ed395b91dfacd1b47fe0545fb5 in /
# Mon, 18 Jul 2016 17:34:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 18 Jul 2016 17:34:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 17:34:57 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Mon, 18 Jul 2016 17:34:58 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2016 19:05:53 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 19:05:56 GMT
RUN locale-gen en_US.UTF-8
# Mon, 18 Jul 2016 19:05:56 GMT
ENV LANG=en_US.UTF-8
# Mon, 18 Jul 2016 19:06:15 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Mon, 18 Jul 2016 19:06:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Mon, 18 Jul 2016 19:07:54 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:08:05 GMT
RUN rosdep init     && rosdep update
# Mon, 18 Jul 2016 19:12:26 GMT
ENV ROS_DISTRO=jade
# Mon, 18 Jul 2016 19:15:02 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-core=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:15:04 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Mon, 18 Jul 2016 19:15:04 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Mon, 18 Jul 2016 19:15:05 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:96c6a1f3c3b0183063a9dad891fe6d8ec466c2fdf9571a0c19b3319ea8a58871`  
		Last Modified: Mon, 18 Jul 2016 17:36:54 GMT  
		Size: 65.7 MB (65699069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4767a2d70a73a271b76a76e4d5edf1426c49ccc24dc7df06ebccd880f01bbeab`  
		Last Modified: Mon, 18 Jul 2016 17:36:35 GMT  
		Size: 92.3 KB (92340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422639bc8a94f4f9ece99c13140bd78b9f25eb62492dd0402ffa4ec58b0d6d9b`  
		Last Modified: Mon, 18 Jul 2016 17:36:35 GMT  
		Size: 366.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a797489a324abb3d09826e5f5a529034aecdc962d54ca4dd642f9548c455295f`  
		Last Modified: Mon, 18 Jul 2016 17:36:35 GMT  
		Size: 682.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6675829cf13b49fb5d7afa4153cc834f0739bc7d25cacd7915bd58e9935da53`  
		Last Modified: Mon, 18 Jul 2016 19:10:54 GMT  
		Size: 329.2 KB (329185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffd474e471fc5604c08bd8925c1e19f391dba9c684ac1e65f4a0141c771b50d`  
		Last Modified: Mon, 18 Jul 2016 19:10:52 GMT  
		Size: 13.1 KB (13071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5645edeaaeed66f0df1c6bd4da8bbb5dd910a67c5323215a36aa8b9468ee9e`  
		Last Modified: Mon, 18 Jul 2016 19:10:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a82b6288ded8b62f1cd6625b1fee4ec208d2cf2f9e79a3ea599359b0c3bbc6`  
		Last Modified: Mon, 18 Jul 2016 19:11:04 GMT  
		Size: 32.9 MB (32870505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ea19c111a704f52c77df988862b9570734510cc71fb2981a640d5f9ecd8d24`  
		Last Modified: Mon, 18 Jul 2016 19:10:50 GMT  
		Size: 630.2 KB (630200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae04cfa9c509c24aa58c4f533f5b8916f295217bf041f86f7e8906a8b1d8b718`  
		Last Modified: Mon, 18 Jul 2016 19:15:57 GMT  
		Size: 150.0 MB (150044762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3552dd371a373bb4881286ebf84425c708bbc1c2c00e23da19307193814fac6d`  
		Last Modified: Mon, 18 Jul 2016 19:15:14 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:jade-ros-base`

```console
$ docker pull ros@sha256:0c2b37d50580fcd8fada507c4ba186a051f21eedfb5311319dcdc5974a0853dd
```

-	Platforms:
	-	linux; amd64

### `ros:jade-ros-base` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.1 MB (253119447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa440cafe9643330e1060c21dd8f7e019fd6dcd789265f4e8528002f054092bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:12:35 GMT
ENV ROS_DISTRO=jade
# Fri, 24 Jun 2016 20:15:07 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-core=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:15:09 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:15:09 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:15:10 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:24:04 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:25:06 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-base=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eb40cd4acd4bea988573bd91ebeaa5f55bc009755f2abd9a51d1d863d332d1`  
		Last Modified: Fri, 24 Jun 2016 20:15:59 GMT  
		Size: 150.0 MB (150047207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1353870c13d5b55b4f4229f17e766ae28dfef6e82a878cfb782b77cd9e9bae`  
		Last Modified: Fri, 24 Jun 2016 20:15:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e97f57f7fb3fc8cb5a7054878cf7224e6f2d68499da13c5e6486cc289ad4089`  
		Last Modified: Wed, 29 Jun 2016 19:25:23 GMT  
		Size: 3.4 MB (3442884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:jade`

```console
$ docker pull ros@sha256:0c2b37d50580fcd8fada507c4ba186a051f21eedfb5311319dcdc5974a0853dd
```

-	Platforms:
	-	linux; amd64

### `ros:jade` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.1 MB (253119447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa440cafe9643330e1060c21dd8f7e019fd6dcd789265f4e8528002f054092bd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:12:35 GMT
ENV ROS_DISTRO=jade
# Fri, 24 Jun 2016 20:15:07 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-core=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:15:09 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:15:09 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:15:10 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:24:04 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:25:06 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-base=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eb40cd4acd4bea988573bd91ebeaa5f55bc009755f2abd9a51d1d863d332d1`  
		Last Modified: Fri, 24 Jun 2016 20:15:59 GMT  
		Size: 150.0 MB (150047207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1353870c13d5b55b4f4229f17e766ae28dfef6e82a878cfb782b77cd9e9bae`  
		Last Modified: Fri, 24 Jun 2016 20:15:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e97f57f7fb3fc8cb5a7054878cf7224e6f2d68499da13c5e6486cc289ad4089`  
		Last Modified: Wed, 29 Jun 2016 19:25:23 GMT  
		Size: 3.4 MB (3442884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:jade-robot`

```console
$ docker pull ros@sha256:8c15823422bddb9d200f0e61fb0b6f3256d9990806393f8a00db23ab31ba8933
```

-	Platforms:
	-	linux; amd64

### `ros:jade-robot` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321162752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7591ddd43afa220fa94f1dee49f5e2396438bccae417ebf65fb2572a0b898f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:12:35 GMT
ENV ROS_DISTRO=jade
# Fri, 24 Jun 2016 20:15:07 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-core=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:15:09 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:15:09 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:15:10 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:24:04 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:25:06 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-base=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:33:05 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:43:26 GMT
RUN apt-get update && apt-get install -y     ros-jade-robot=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eb40cd4acd4bea988573bd91ebeaa5f55bc009755f2abd9a51d1d863d332d1`  
		Last Modified: Fri, 24 Jun 2016 20:15:59 GMT  
		Size: 150.0 MB (150047207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1353870c13d5b55b4f4229f17e766ae28dfef6e82a878cfb782b77cd9e9bae`  
		Last Modified: Fri, 24 Jun 2016 20:15:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e97f57f7fb3fc8cb5a7054878cf7224e6f2d68499da13c5e6486cc289ad4089`  
		Last Modified: Wed, 29 Jun 2016 19:25:23 GMT  
		Size: 3.4 MB (3442884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a10e7b916cf28132610ab07615aab228fefccc269cd7fd85dad448de111857a`  
		Last Modified: Fri, 08 Jul 2016 19:44:08 GMT  
		Size: 68.0 MB (68043305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:jade-perception`

```console
$ docker pull ros@sha256:6938e8519007989125fe4d1c803763a1291f7a07ef4d08488c83cc4171b17a83
```

-	Platforms:
	-	linux; amd64

### `ros:jade-perception` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **520.7 MB (520706892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42181a2cbb188a6f27536e094d64933a1f41b8b4d91d36c6109149041e0d5d13`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 24 Jun 2016 17:29:06 GMT
ADD file:b6ff401cf2a7a08c11d2bdfbfec31c7ec105fd7ab29c529fb90025762b077e2c in /
# Fri, 24 Jun 2016 17:29:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 24 Jun 2016 17:29:11 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 17:29:13 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 24 Jun 2016 17:29:14 GMT
CMD ["/bin/bash"]
# Fri, 24 Jun 2016 20:03:46 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 24 Jun 2016 20:03:49 GMT
RUN locale-gen en_US.UTF-8
# Fri, 24 Jun 2016 20:03:49 GMT
ENV LANG=en_US.UTF-8
# Fri, 24 Jun 2016 20:04:07 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 24 Jun 2016 20:04:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu trusty main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 24 Jun 2016 20:05:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:05:58 GMT
RUN rosdep init     && rosdep update
# Fri, 24 Jun 2016 20:12:35 GMT
ENV ROS_DISTRO=jade
# Fri, 24 Jun 2016 20:15:07 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-core=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2016 20:15:09 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 24 Jun 2016 20:15:09 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 24 Jun 2016 20:15:10 GMT
CMD ["bash"]
# Wed, 29 Jun 2016 19:24:04 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Wed, 29 Jun 2016 19:25:06 GMT
RUN apt-get update && apt-get install -y     ros-jade-ros-base=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:33:05 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:39:01 GMT
RUN apt-get update && apt-get install -y     ros-jade-perception=1.2.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56eb14001cebec19f2255d95e125c9f5199c9e1d97dd708e1f3ebda3d32e5da7`  
		Last Modified: Fri, 24 Jun 2016 17:30:48 GMT  
		Size: 65.7 MB (65699368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff49c327d838cf14f7db33fa44f6057b7209298e9c03369257485a085e231df`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 101.4 KB (101415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e532f87f96dd5821006d02e65e7d4729a4e6957a34c3f4ec72046e221eb7c52`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce63537e70c2c250fbc41b5f04bfb31f445be4034effc4b4c513bf8899dfa0a`  
		Last Modified: Fri, 24 Jun 2016 17:30:29 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6651aae8bc83a7cb9dc7544adeefe81369a70d5df8fd7733a78789ef2c32f3`  
		Last Modified: Fri, 24 Jun 2016 20:08:43 GMT  
		Size: 329.2 KB (329188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a831e99b405d8c6a12dbbf9a600d35e19f9da13396bfc759c13cfb08c65dfa`  
		Last Modified: Fri, 24 Jun 2016 20:08:42 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd005d0940c11d0c40900ba072adf2bb26a2f5200ab54b45a78a1f2b643ad4`  
		Last Modified: Fri, 24 Jun 2016 20:08:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800815708586712669e2761b3b81962327e2e1e48ee479e7a6d1fb3bcfad0f24`  
		Last Modified: Fri, 24 Jun 2016 20:08:51 GMT  
		Size: 32.9 MB (32870801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5c3ed1ff87ca2b6011c1726fe0b9e1301fa6ea26a94c29bbd67f278b13ed9`  
		Last Modified: Fri, 24 Jun 2016 20:08:40 GMT  
		Size: 614.0 KB (614050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77eb40cd4acd4bea988573bd91ebeaa5f55bc009755f2abd9a51d1d863d332d1`  
		Last Modified: Fri, 24 Jun 2016 20:15:59 GMT  
		Size: 150.0 MB (150047207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1353870c13d5b55b4f4229f17e766ae28dfef6e82a878cfb782b77cd9e9bae`  
		Last Modified: Fri, 24 Jun 2016 20:15:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e97f57f7fb3fc8cb5a7054878cf7224e6f2d68499da13c5e6486cc289ad4089`  
		Last Modified: Wed, 29 Jun 2016 19:25:23 GMT  
		Size: 3.4 MB (3442884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3e34105b1076146407c427f0b3dcca9d5f8447b00949ea5746def8b8c675e1`  
		Last Modified: Fri, 08 Jul 2016 19:40:43 GMT  
		Size: 267.6 MB (267587445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-core`

```console
$ docker pull ros@sha256:c44a7c030160f3fe4e9bf27eb393bc14e5ddce55be8c61397f5e4906c2aa244c
```

-	Platforms:
	-	linux; amd64

### `ros:kinetic-ros-core` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297653054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0bb7be7c83283a4b3878ad77ae16bcc8ce3c196feb35bcd41667297078526b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 18 Jul 2016 17:35:22 GMT
ADD file:fdbd881d78f9d7d9245d0838389ebc793bef13243b9e3269512046cd75216baf in /
# Mon, 18 Jul 2016 17:35:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 18 Jul 2016 17:35:26 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 17:35:27 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Mon, 18 Jul 2016 17:35:28 GMT
CMD ["/bin/bash"]
# Mon, 18 Jul 2016 19:00:44 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 19:00:47 GMT
RUN locale-gen en_US.UTF-8
# Mon, 18 Jul 2016 19:00:48 GMT
ENV LANG=en_US.UTF-8
# Mon, 18 Jul 2016 19:00:52 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Mon, 18 Jul 2016 19:00:53 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Mon, 18 Jul 2016 19:01:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:02:09 GMT
RUN rosdep init     && rosdep update
# Mon, 18 Jul 2016 19:02:10 GMT
ENV ROS_DISTRO=kinetic
# Mon, 18 Jul 2016 19:03:52 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:03:55 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Mon, 18 Jul 2016 19:03:56 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Mon, 18 Jul 2016 19:03:56 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:43db9dbdcb300fc39b23e88a1721bdaa95c7fe396bd89d6a4b1a39e8da1a2d4c`  
		Last Modified: Mon, 18 Jul 2016 17:38:23 GMT  
		Size: 49.3 MB (49325555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a9cd1fcca227737b80281fed1c60453a7a49b02a956bb6531276df5646e77e`  
		Last Modified: Mon, 18 Jul 2016 17:38:09 GMT  
		Size: 21.7 KB (21651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23af84961027ee5a7725040d44b30d563eb6a79f013d2c924e31cae43367f33`  
		Last Modified: Mon, 18 Jul 2016 17:38:09 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88c36ca55d86a9331db93eef6dcac6a7027c19205fdb706185703ef28db154e`  
		Last Modified: Mon, 18 Jul 2016 17:38:09 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22aac2bec911aff1c1ff2fd216be2f54cf21bf8ae3806a73db8f1e7b2132e635`  
		Last Modified: Mon, 18 Jul 2016 19:04:08 GMT  
		Size: 339.4 KB (339413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b333626c9f13b55787e210260bf2b62031a39a5754ba97a5c993f33ec9e8a171`  
		Last Modified: Mon, 18 Jul 2016 19:04:08 GMT  
		Size: 13.1 KB (13070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193d40022f088e58d6b742066e9ae1c878040e0a5ddc220821c848ac22274699`  
		Last Modified: Mon, 18 Jul 2016 19:04:05 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a2f175e052baefc7ba8a05b07038cf6f9b381de17210dd203ca3e992fb2970`  
		Last Modified: Mon, 18 Jul 2016 19:04:27 GMT  
		Size: 57.7 MB (57681476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b6b5ac0b0f6b51be47f6d82280b62cd7f7664c52f09400444c36541ca50c0d`  
		Last Modified: Mon, 18 Jul 2016 19:04:05 GMT  
		Size: 630.2 KB (630209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e64def3891e6e50e0dcd6e6b037b352833b871ac63a5da0dea98817c3c26683`  
		Last Modified: Mon, 18 Jul 2016 19:05:01 GMT  
		Size: 189.6 MB (189640132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca2d13565db66c95c4f77169f7633ebc7375ac1911a2d3f0a989e693f32a8cc`  
		Last Modified: Mon, 18 Jul 2016 19:04:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-ros-base`

```console
$ docker pull ros@sha256:0ca176612ca2c1919e384e543e33be2cda40a44b01624f9c894359fd9e3cb088
```

-	Platforms:
	-	linux; amd64

### `ros:kinetic-ros-base` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302169370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf95391def349a023463bfaf495e1d80c5b2b936fbc55dcbaea1320db663fb6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 08 Jul 2016 18:39:36 GMT
ADD file:49ae6eed5178a2866c5023c4e7a9ae303f4828a5586569106aff27a8ce9cadf6 in /
# Fri, 08 Jul 2016 18:39:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 08 Jul 2016 18:39:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 18:39:43 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 08 Jul 2016 18:39:43 GMT
CMD ["/bin/bash"]
# Fri, 08 Jul 2016 19:22:51 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:22:54 GMT
RUN locale-gen en_US.UTF-8
# Fri, 08 Jul 2016 19:22:55 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Jul 2016 19:22:59 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 08 Jul 2016 19:23:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 08 Jul 2016 19:24:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:24:45 GMT
RUN rosdep init     && rosdep update
# Fri, 08 Jul 2016 19:24:46 GMT
ENV ROS_DISTRO=kinetic
# Fri, 08 Jul 2016 19:27:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:27:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 08 Jul 2016 19:27:14 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 08 Jul 2016 19:27:15 GMT
CMD ["bash"]
# Mon, 18 Jul 2016 18:59:42 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 18:59:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90d6565b970a2a27b197806e3a2bd19cc0fd1fc9241f7c00ae2f1295b3cac38d`  
		Last Modified: Thu, 07 Jul 2016 12:52:32 GMT  
		Size: 49.3 MB (49257890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40553bdb84743dd9a3216ab110d274a01e309b916b3c628525a255969c6bdd61`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 21.6 KB (21556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3129e7479abf3d666ac61caefdb62d03bfbd0f322f01d1f8bf30633a98c1bb8`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091663bd70db6ceba4405547c1e143f8ef676910aa914fe9edd87340cd3742b4`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b369ebb1884ce3e37307341d708ae158a77d97d6f011a2dccb1d76048e03a0`  
		Last Modified: Fri, 08 Jul 2016 19:27:27 GMT  
		Size: 339.4 KB (339413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e1ca03689ea489b2d4b9594b4d46f3c1c592657c91884fba84f856efc5fed`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 13.1 KB (13072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9755ad6b38c49ef9ad0eaa50cf7f64478de073a689f3085fb8463e6c313bbbff`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d5c1cb01c8239326c60d54243f34beefa50bc2ba1259fdb596edadeebbe291`  
		Last Modified: Fri, 08 Jul 2016 19:27:51 GMT  
		Size: 57.6 MB (57585769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e25bd4b2228a9307dbf047cbfcac7603b8b33549e2b05932023593087a8650c`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 624.1 KB (624125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aee8140ec59014b431af136aa95b4a2a7a031873d0f2175a55759e192c1e32`  
		Last Modified: Fri, 08 Jul 2016 19:28:49 GMT  
		Size: 189.7 MB (189658103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4890924e9c3f083be453fdfa4292a7b4a5fe8bcc15e3de7fde200a4fae812a`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92258fc5a678453624224a0bd83dbb6db00190a23a26633a45f9f2799b7f4d0e`  
		Last Modified: Mon, 18 Jul 2016 19:00:09 GMT  
		Size: 4.7 MB (4667901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic`

```console
$ docker pull ros@sha256:0ca176612ca2c1919e384e543e33be2cda40a44b01624f9c894359fd9e3cb088
```

-	Platforms:
	-	linux; amd64

### `ros:kinetic` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302169370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf95391def349a023463bfaf495e1d80c5b2b936fbc55dcbaea1320db663fb6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 08 Jul 2016 18:39:36 GMT
ADD file:49ae6eed5178a2866c5023c4e7a9ae303f4828a5586569106aff27a8ce9cadf6 in /
# Fri, 08 Jul 2016 18:39:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 08 Jul 2016 18:39:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 18:39:43 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 08 Jul 2016 18:39:43 GMT
CMD ["/bin/bash"]
# Fri, 08 Jul 2016 19:22:51 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:22:54 GMT
RUN locale-gen en_US.UTF-8
# Fri, 08 Jul 2016 19:22:55 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Jul 2016 19:22:59 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 08 Jul 2016 19:23:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 08 Jul 2016 19:24:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:24:45 GMT
RUN rosdep init     && rosdep update
# Fri, 08 Jul 2016 19:24:46 GMT
ENV ROS_DISTRO=kinetic
# Fri, 08 Jul 2016 19:27:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:27:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 08 Jul 2016 19:27:14 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 08 Jul 2016 19:27:15 GMT
CMD ["bash"]
# Mon, 18 Jul 2016 18:59:42 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 18:59:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90d6565b970a2a27b197806e3a2bd19cc0fd1fc9241f7c00ae2f1295b3cac38d`  
		Last Modified: Thu, 07 Jul 2016 12:52:32 GMT  
		Size: 49.3 MB (49257890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40553bdb84743dd9a3216ab110d274a01e309b916b3c628525a255969c6bdd61`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 21.6 KB (21556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3129e7479abf3d666ac61caefdb62d03bfbd0f322f01d1f8bf30633a98c1bb8`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091663bd70db6ceba4405547c1e143f8ef676910aa914fe9edd87340cd3742b4`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b369ebb1884ce3e37307341d708ae158a77d97d6f011a2dccb1d76048e03a0`  
		Last Modified: Fri, 08 Jul 2016 19:27:27 GMT  
		Size: 339.4 KB (339413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e1ca03689ea489b2d4b9594b4d46f3c1c592657c91884fba84f856efc5fed`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 13.1 KB (13072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9755ad6b38c49ef9ad0eaa50cf7f64478de073a689f3085fb8463e6c313bbbff`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d5c1cb01c8239326c60d54243f34beefa50bc2ba1259fdb596edadeebbe291`  
		Last Modified: Fri, 08 Jul 2016 19:27:51 GMT  
		Size: 57.6 MB (57585769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e25bd4b2228a9307dbf047cbfcac7603b8b33549e2b05932023593087a8650c`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 624.1 KB (624125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aee8140ec59014b431af136aa95b4a2a7a031873d0f2175a55759e192c1e32`  
		Last Modified: Fri, 08 Jul 2016 19:28:49 GMT  
		Size: 189.7 MB (189658103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4890924e9c3f083be453fdfa4292a7b4a5fe8bcc15e3de7fde200a4fae812a`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92258fc5a678453624224a0bd83dbb6db00190a23a26633a45f9f2799b7f4d0e`  
		Last Modified: Mon, 18 Jul 2016 19:00:09 GMT  
		Size: 4.7 MB (4667901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:latest`

```console
$ docker pull ros@sha256:0ca176612ca2c1919e384e543e33be2cda40a44b01624f9c894359fd9e3cb088
```

-	Platforms:
	-	linux; amd64

### `ros:latest` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302169370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf95391def349a023463bfaf495e1d80c5b2b936fbc55dcbaea1320db663fb6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 08 Jul 2016 18:39:36 GMT
ADD file:49ae6eed5178a2866c5023c4e7a9ae303f4828a5586569106aff27a8ce9cadf6 in /
# Fri, 08 Jul 2016 18:39:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 08 Jul 2016 18:39:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 18:39:43 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 08 Jul 2016 18:39:43 GMT
CMD ["/bin/bash"]
# Fri, 08 Jul 2016 19:22:51 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:22:54 GMT
RUN locale-gen en_US.UTF-8
# Fri, 08 Jul 2016 19:22:55 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Jul 2016 19:22:59 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 08 Jul 2016 19:23:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 08 Jul 2016 19:24:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:24:45 GMT
RUN rosdep init     && rosdep update
# Fri, 08 Jul 2016 19:24:46 GMT
ENV ROS_DISTRO=kinetic
# Fri, 08 Jul 2016 19:27:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:27:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 08 Jul 2016 19:27:14 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 08 Jul 2016 19:27:15 GMT
CMD ["bash"]
# Mon, 18 Jul 2016 18:59:42 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 18:59:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90d6565b970a2a27b197806e3a2bd19cc0fd1fc9241f7c00ae2f1295b3cac38d`  
		Last Modified: Thu, 07 Jul 2016 12:52:32 GMT  
		Size: 49.3 MB (49257890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40553bdb84743dd9a3216ab110d274a01e309b916b3c628525a255969c6bdd61`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 21.6 KB (21556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3129e7479abf3d666ac61caefdb62d03bfbd0f322f01d1f8bf30633a98c1bb8`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091663bd70db6ceba4405547c1e143f8ef676910aa914fe9edd87340cd3742b4`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b369ebb1884ce3e37307341d708ae158a77d97d6f011a2dccb1d76048e03a0`  
		Last Modified: Fri, 08 Jul 2016 19:27:27 GMT  
		Size: 339.4 KB (339413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e1ca03689ea489b2d4b9594b4d46f3c1c592657c91884fba84f856efc5fed`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 13.1 KB (13072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9755ad6b38c49ef9ad0eaa50cf7f64478de073a689f3085fb8463e6c313bbbff`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d5c1cb01c8239326c60d54243f34beefa50bc2ba1259fdb596edadeebbe291`  
		Last Modified: Fri, 08 Jul 2016 19:27:51 GMT  
		Size: 57.6 MB (57585769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e25bd4b2228a9307dbf047cbfcac7603b8b33549e2b05932023593087a8650c`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 624.1 KB (624125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aee8140ec59014b431af136aa95b4a2a7a031873d0f2175a55759e192c1e32`  
		Last Modified: Fri, 08 Jul 2016 19:28:49 GMT  
		Size: 189.7 MB (189658103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4890924e9c3f083be453fdfa4292a7b4a5fe8bcc15e3de7fde200a4fae812a`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92258fc5a678453624224a0bd83dbb6db00190a23a26633a45f9f2799b7f4d0e`  
		Last Modified: Mon, 18 Jul 2016 19:00:09 GMT  
		Size: 4.7 MB (4667901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-robot`

```console
$ docker pull ros@sha256:3a6f3c344387387e61d27b253587db77a10fd91cf041eeb7fd24d0d2a49cbcda
```

-	Platforms:
	-	linux; amd64

### `ros:kinetic-robot` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.5 MB (442457390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e240fafacfc4dcedfa8494358c2a4b43c296c8b79941f4d589af1f9728d41e`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 08 Jul 2016 18:39:36 GMT
ADD file:49ae6eed5178a2866c5023c4e7a9ae303f4828a5586569106aff27a8ce9cadf6 in /
# Fri, 08 Jul 2016 18:39:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 08 Jul 2016 18:39:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 18:39:43 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 08 Jul 2016 18:39:43 GMT
CMD ["/bin/bash"]
# Fri, 08 Jul 2016 19:22:51 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:22:54 GMT
RUN locale-gen en_US.UTF-8
# Fri, 08 Jul 2016 19:22:55 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Jul 2016 19:22:59 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 08 Jul 2016 19:23:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 08 Jul 2016 19:24:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:24:45 GMT
RUN rosdep init     && rosdep update
# Fri, 08 Jul 2016 19:24:46 GMT
ENV ROS_DISTRO=kinetic
# Fri, 08 Jul 2016 19:27:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:27:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 08 Jul 2016 19:27:14 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 08 Jul 2016 19:27:15 GMT
CMD ["bash"]
# Mon, 18 Jul 2016 18:59:42 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 18:59:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:16:11 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 19:24:25 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-robot=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90d6565b970a2a27b197806e3a2bd19cc0fd1fc9241f7c00ae2f1295b3cac38d`  
		Last Modified: Thu, 07 Jul 2016 12:52:32 GMT  
		Size: 49.3 MB (49257890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40553bdb84743dd9a3216ab110d274a01e309b916b3c628525a255969c6bdd61`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 21.6 KB (21556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3129e7479abf3d666ac61caefdb62d03bfbd0f322f01d1f8bf30633a98c1bb8`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091663bd70db6ceba4405547c1e143f8ef676910aa914fe9edd87340cd3742b4`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b369ebb1884ce3e37307341d708ae158a77d97d6f011a2dccb1d76048e03a0`  
		Last Modified: Fri, 08 Jul 2016 19:27:27 GMT  
		Size: 339.4 KB (339413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e1ca03689ea489b2d4b9594b4d46f3c1c592657c91884fba84f856efc5fed`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 13.1 KB (13072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9755ad6b38c49ef9ad0eaa50cf7f64478de073a689f3085fb8463e6c313bbbff`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d5c1cb01c8239326c60d54243f34beefa50bc2ba1259fdb596edadeebbe291`  
		Last Modified: Fri, 08 Jul 2016 19:27:51 GMT  
		Size: 57.6 MB (57585769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e25bd4b2228a9307dbf047cbfcac7603b8b33549e2b05932023593087a8650c`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 624.1 KB (624125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aee8140ec59014b431af136aa95b4a2a7a031873d0f2175a55759e192c1e32`  
		Last Modified: Fri, 08 Jul 2016 19:28:49 GMT  
		Size: 189.7 MB (189658103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4890924e9c3f083be453fdfa4292a7b4a5fe8bcc15e3de7fde200a4fae812a`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92258fc5a678453624224a0bd83dbb6db00190a23a26633a45f9f2799b7f4d0e`  
		Last Modified: Mon, 18 Jul 2016 19:00:09 GMT  
		Size: 4.7 MB (4667901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fd69150a44cb9d7f2dc7beb1cb3b80bfdf2a0f0de6fa883cb90bed8329e50c`  
		Last Modified: Mon, 18 Jul 2016 19:25:15 GMT  
		Size: 140.3 MB (140288020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ros:kinetic-perception`

```console
$ docker pull ros@sha256:d527bef677e400e09e4cf6aaf38779f2f99f297ecab47dbef3e06dbb00de07c7
```

-	Platforms:
	-	linux; amd64

### `ros:kinetic-perception` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **705.8 MB (705773500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88ccf2a6bf1a02bf474d9a0185bf34d44046e21ce172d0fa6801289acc51a848`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 08 Jul 2016 18:39:36 GMT
ADD file:49ae6eed5178a2866c5023c4e7a9ae303f4828a5586569106aff27a8ce9cadf6 in /
# Fri, 08 Jul 2016 18:39:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes
# Fri, 08 Jul 2016 18:39:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 18:39:43 GMT
RUN sed -i 's/^#\s*\(deb.*universe\)$/\1/g' /etc/apt/sources.list
# Fri, 08 Jul 2016 18:39:43 GMT
CMD ["/bin/bash"]
# Fri, 08 Jul 2016 19:22:51 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Fri, 08 Jul 2016 19:22:54 GMT
RUN locale-gen en_US.UTF-8
# Fri, 08 Jul 2016 19:22:55 GMT
ENV LANG=en_US.UTF-8
# Fri, 08 Jul 2016 19:22:59 GMT
RUN apt-key adv --keyserver ha.pool.sks-keyservers.net --recv-keys 421C365BD9FF1F717815A3895523BAEEB01FA116
# Fri, 08 Jul 2016 19:23:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list
# Fri, 08 Jul 2016 19:24:25 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:24:45 GMT
RUN rosdep init     && rosdep update
# Fri, 08 Jul 2016 19:24:46 GMT
ENV ROS_DISTRO=kinetic
# Fri, 08 Jul 2016 19:27:11 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-core=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Jul 2016 19:27:14 GMT
COPY file:824303428ad16ae6296df253434e00a00126dc8404f740a8b885c9f61a2f5fcb in /
# Fri, 08 Jul 2016 19:27:14 GMT
ENTRYPOINT &{["/ros_entrypoint.sh"]}
# Fri, 08 Jul 2016 19:27:15 GMT
CMD ["bash"]
# Mon, 18 Jul 2016 18:59:42 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 18:59:59 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-ros-base=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 18 Jul 2016 19:16:11 GMT
MAINTAINER Tully Foote tfoote+buildfarm@osrfoundation.org
# Mon, 18 Jul 2016 19:20:17 GMT
RUN apt-get update && apt-get install -y     ros-kinetic-perception=1.3.0-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:90d6565b970a2a27b197806e3a2bd19cc0fd1fc9241f7c00ae2f1295b3cac38d`  
		Last Modified: Thu, 07 Jul 2016 12:52:32 GMT  
		Size: 49.3 MB (49257890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40553bdb84743dd9a3216ab110d274a01e309b916b3c628525a255969c6bdd61`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 21.6 KB (21556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3129e7479abf3d666ac61caefdb62d03bfbd0f322f01d1f8bf30633a98c1bb8`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091663bd70db6ceba4405547c1e143f8ef676910aa914fe9edd87340cd3742b4`  
		Last Modified: Fri, 08 Jul 2016 18:42:37 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b369ebb1884ce3e37307341d708ae158a77d97d6f011a2dccb1d76048e03a0`  
		Last Modified: Fri, 08 Jul 2016 19:27:27 GMT  
		Size: 339.4 KB (339413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651e1ca03689ea489b2d4b9594b4d46f3c1c592657c91884fba84f856efc5fed`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 13.1 KB (13072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9755ad6b38c49ef9ad0eaa50cf7f64478de073a689f3085fb8463e6c313bbbff`  
		Last Modified: Fri, 08 Jul 2016 19:27:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d5c1cb01c8239326c60d54243f34beefa50bc2ba1259fdb596edadeebbe291`  
		Last Modified: Fri, 08 Jul 2016 19:27:51 GMT  
		Size: 57.6 MB (57585769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e25bd4b2228a9307dbf047cbfcac7603b8b33549e2b05932023593087a8650c`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 624.1 KB (624125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aee8140ec59014b431af136aa95b4a2a7a031873d0f2175a55759e192c1e32`  
		Last Modified: Fri, 08 Jul 2016 19:28:49 GMT  
		Size: 189.7 MB (189658103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4890924e9c3f083be453fdfa4292a7b4a5fe8bcc15e3de7fde200a4fae812a`  
		Last Modified: Fri, 08 Jul 2016 19:27:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92258fc5a678453624224a0bd83dbb6db00190a23a26633a45f9f2799b7f4d0e`  
		Last Modified: Mon, 18 Jul 2016 19:00:09 GMT  
		Size: 4.7 MB (4667901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a3eeb529e48e9b6e2e8c261615c0d8a0230873bcde2182212eacd454c218a0`  
		Last Modified: Mon, 18 Jul 2016 19:22:28 GMT  
		Size: 403.6 MB (403604130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
