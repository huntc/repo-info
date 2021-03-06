<!-- THIS FILE IS GENERATED VIA './update-tag-details.sh' -->

# Tags of `golang`

-	[`golang:1.6.3`](#golang163)
-	[`golang:1.6`](#golang16)
-	[`golang:1.6.3-onbuild`](#golang163-onbuild)
-	[`golang:1.6-onbuild`](#golang16-onbuild)
-	[`golang:1.6.3-wheezy`](#golang163-wheezy)
-	[`golang:1.6-wheezy`](#golang16-wheezy)
-	[`golang:1.6.3-alpine`](#golang163-alpine)
-	[`golang:1.6-alpine`](#golang16-alpine)
-	[`golang:1.6.3-windowsservercore`](#golang163-windowsservercore)
-	[`golang:1.6-windowsservercore`](#golang16-windowsservercore)
-	[`golang:1.7.0`](#golang170)
-	[`golang:1.7`](#golang17)
-	[`golang:1`](#golang1)
-	[`golang:latest`](#golanglatest)
-	[`golang:1.7.0-onbuild`](#golang170-onbuild)
-	[`golang:1.7-onbuild`](#golang17-onbuild)
-	[`golang:1-onbuild`](#golang1-onbuild)
-	[`golang:onbuild`](#golangonbuild)
-	[`golang:1.7.0-wheezy`](#golang170-wheezy)
-	[`golang:1.7-wheezy`](#golang17-wheezy)
-	[`golang:1-wheezy`](#golang1-wheezy)
-	[`golang:wheezy`](#golangwheezy)
-	[`golang:1.7.0-alpine`](#golang170-alpine)
-	[`golang:1.7-alpine`](#golang17-alpine)
-	[`golang:1-alpine`](#golang1-alpine)
-	[`golang:alpine`](#golangalpine)
-	[`golang:1.7.0-windowsservercore`](#golang170-windowsservercore)
-	[`golang:1.7-windowsservercore`](#golang17-windowsservercore)
-	[`golang:1-windowsservercore`](#golang1-windowsservercore)
-	[`golang:windowsservercore`](#golangwindowsservercore)

## `golang:1.6.3`

```console
$ docker pull golang@sha256:247a91a8a6a3038f2ba422ead03339eb736f427e08175272f054722f9f2aac51
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.2 MB (254163199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24c8478ed407db5bf9c4efd0773fe75975b2bc321dd8f0ab1e42a898fcb6ea4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 04:02:22 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 29 Jul 2016 04:02:35 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 29 Jul 2016 04:02:36 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2016 04:02:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2016 04:02:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2016 04:02:39 GMT
WORKDIR /go
# Fri, 29 Jul 2016 04:02:41 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85155ee2fbc2368de761d83d22f770d917b254ee04164f8c1c1b21a940d4e24f`  
		Last Modified: Fri, 29 Jul 2016 04:03:16 GMT  
		Size: 84.9 MB (84869285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51febe8479886dbe081dce679513ae53af598918d629356cfb1982ca1cb3a63`  
		Last Modified: Fri, 29 Jul 2016 04:02:51 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52609aaab90b1923cc0e2ab262d2121b4ca5fbc65ab5ecee493d953663207a4a`  
		Last Modified: Fri, 29 Jul 2016 04:02:49 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6`

```console
$ docker pull golang@sha256:247a91a8a6a3038f2ba422ead03339eb736f427e08175272f054722f9f2aac51
```

-	Platforms:
	-	linux; amd64

### `golang:1.6` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.2 MB (254163199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24c8478ed407db5bf9c4efd0773fe75975b2bc321dd8f0ab1e42a898fcb6ea4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 04:02:22 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 29 Jul 2016 04:02:35 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 29 Jul 2016 04:02:36 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2016 04:02:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2016 04:02:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2016 04:02:39 GMT
WORKDIR /go
# Fri, 29 Jul 2016 04:02:41 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85155ee2fbc2368de761d83d22f770d917b254ee04164f8c1c1b21a940d4e24f`  
		Last Modified: Fri, 29 Jul 2016 04:03:16 GMT  
		Size: 84.9 MB (84869285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51febe8479886dbe081dce679513ae53af598918d629356cfb1982ca1cb3a63`  
		Last Modified: Fri, 29 Jul 2016 04:02:51 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52609aaab90b1923cc0e2ab262d2121b4ca5fbc65ab5ecee493d953663207a4a`  
		Last Modified: Fri, 29 Jul 2016 04:02:49 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-onbuild`

```console
$ docker pull golang@sha256:13429695826de16054729d6f32b8cc1dc5d0d46116774fb3a22d06e19a900756
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3-onbuild` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.2 MB (254163329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f38868dbb9c15368c299aa5820595c7016781923024731e1a73ab194b2121d3`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 04:02:22 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 29 Jul 2016 04:02:35 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 29 Jul 2016 04:02:36 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2016 04:02:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2016 04:02:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2016 04:02:39 GMT
WORKDIR /go
# Fri, 29 Jul 2016 04:02:41 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
# Fri, 29 Jul 2016 04:03:54 GMT
RUN mkdir -p /go/src/app
# Fri, 29 Jul 2016 04:03:55 GMT
WORKDIR /go/src/app
# Fri, 29 Jul 2016 04:03:55 GMT
CMD ["go-wrapper" "run"]
# Fri, 29 Jul 2016 04:03:56 GMT
ONBUILD COPY . /go/src/app
# Fri, 29 Jul 2016 04:03:57 GMT
ONBUILD RUN go-wrapper download
# Fri, 29 Jul 2016 04:03:57 GMT
ONBUILD RUN go-wrapper install
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85155ee2fbc2368de761d83d22f770d917b254ee04164f8c1c1b21a940d4e24f`  
		Last Modified: Fri, 29 Jul 2016 04:03:16 GMT  
		Size: 84.9 MB (84869285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51febe8479886dbe081dce679513ae53af598918d629356cfb1982ca1cb3a63`  
		Last Modified: Fri, 29 Jul 2016 04:02:51 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52609aaab90b1923cc0e2ab262d2121b4ca5fbc65ab5ecee493d953663207a4a`  
		Last Modified: Fri, 29 Jul 2016 04:02:49 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebeaceb1f7908bd28e0dd9b162737488d26b0bcaa99c40363112f98d012fc889`  
		Last Modified: Fri, 29 Jul 2016 04:04:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-onbuild`

```console
$ docker pull golang@sha256:13429695826de16054729d6f32b8cc1dc5d0d46116774fb3a22d06e19a900756
```

-	Platforms:
	-	linux; amd64

### `golang:1.6-onbuild` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.2 MB (254163329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f38868dbb9c15368c299aa5820595c7016781923024731e1a73ab194b2121d3`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 04:02:22 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 29 Jul 2016 04:02:23 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 29 Jul 2016 04:02:35 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 29 Jul 2016 04:02:36 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2016 04:02:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2016 04:02:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2016 04:02:39 GMT
WORKDIR /go
# Fri, 29 Jul 2016 04:02:41 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
# Fri, 29 Jul 2016 04:03:54 GMT
RUN mkdir -p /go/src/app
# Fri, 29 Jul 2016 04:03:55 GMT
WORKDIR /go/src/app
# Fri, 29 Jul 2016 04:03:55 GMT
CMD ["go-wrapper" "run"]
# Fri, 29 Jul 2016 04:03:56 GMT
ONBUILD COPY . /go/src/app
# Fri, 29 Jul 2016 04:03:57 GMT
ONBUILD RUN go-wrapper download
# Fri, 29 Jul 2016 04:03:57 GMT
ONBUILD RUN go-wrapper install
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85155ee2fbc2368de761d83d22f770d917b254ee04164f8c1c1b21a940d4e24f`  
		Last Modified: Fri, 29 Jul 2016 04:03:16 GMT  
		Size: 84.9 MB (84869285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51febe8479886dbe081dce679513ae53af598918d629356cfb1982ca1cb3a63`  
		Last Modified: Fri, 29 Jul 2016 04:02:51 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52609aaab90b1923cc0e2ab262d2121b4ca5fbc65ab5ecee493d953663207a4a`  
		Last Modified: Fri, 29 Jul 2016 04:02:49 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebeaceb1f7908bd28e0dd9b162737488d26b0bcaa99c40363112f98d012fc889`  
		Last Modified: Fri, 29 Jul 2016 04:04:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-wheezy`

```console
$ docker pull golang@sha256:1eb0fa3e5054c624fa1fbbf29821d61032e143c3fada528bce10da1b116d0a03
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3-wheezy` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.6 MB (201648625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e86435b53ef6cd9c62ff49c5b3562544fb0b657ac2a91ae77a2262cc7b4fa8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:49:29 GMT
ADD file:0d2a68d1c5a4a52b0bddd8921fe9f3d603a5d69911d4bba61c5e2460e6500d76 in /
# Thu, 28 Jul 2016 17:49:29 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 18:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 18:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 04:04:40 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 29 Jul 2016 04:04:41 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 29 Jul 2016 04:04:42 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 29 Jul 2016 04:04:54 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 29 Jul 2016 04:04:55 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2016 04:04:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2016 04:04:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2016 04:04:58 GMT
WORKDIR /go
# Fri, 29 Jul 2016 04:04:59 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:5c68a10e9f3f9e2757d1f2b0a51ad5ac41f5395a190bbbe3907a6b6fffa9bcea`  
		Last Modified: Thu, 28 Jul 2016 17:54:32 GMT  
		Size: 37.2 MB (37209635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81f9b5104e75c51d678d80525193ab71008b9c25c1a1e4694996b0744c6cbe`  
		Last Modified: Thu, 28 Jul 2016 21:53:17 GMT  
		Size: 6.7 MB (6730996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d9d9752348fab5a9cd1140f31df8ad6ce301aca3e7d4e303d14fde010ea14`  
		Last Modified: Thu, 28 Jul 2016 21:53:49 GMT  
		Size: 38.9 MB (38887392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0238af288e95b46257dcfbe2c650681a0ee6b66bdcf2306ece99f93f1ad794a3`  
		Last Modified: Fri, 29 Jul 2016 03:59:40 GMT  
		Size: 33.9 MB (33949794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453a6a1a4ddc150932047bf9dbfe3b08491372c0de9f889cb58a52e27ea24fbb`  
		Last Modified: Fri, 29 Jul 2016 04:05:37 GMT  
		Size: 84.9 MB (84869331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5ca97ed864658a34e725252086c9b253532062ed97506971694100a94b036e`  
		Last Modified: Fri, 29 Jul 2016 04:05:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b991788ec96628f1f3866f0aab6726922665d5aa247bc8379ca501fc699430c`  
		Last Modified: Fri, 29 Jul 2016 04:05:08 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-wheezy`

```console
$ docker pull golang@sha256:1eb0fa3e5054c624fa1fbbf29821d61032e143c3fada528bce10da1b116d0a03
```

-	Platforms:
	-	linux; amd64

### `golang:1.6-wheezy` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.6 MB (201648625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8e86435b53ef6cd9c62ff49c5b3562544fb0b657ac2a91ae77a2262cc7b4fa8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:49:29 GMT
ADD file:0d2a68d1c5a4a52b0bddd8921fe9f3d603a5d69911d4bba61c5e2460e6500d76 in /
# Thu, 28 Jul 2016 17:49:29 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 18:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 18:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 04:04:40 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 29 Jul 2016 04:04:41 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.linux-amd64.tar.gz
# Fri, 29 Jul 2016 04:04:42 GMT
ENV GOLANG_DOWNLOAD_SHA256=cdde5e08530c0579255d6153b08fdb3b8e47caabbe717bc7bcd7561275a87aeb
# Fri, 29 Jul 2016 04:04:54 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Fri, 29 Jul 2016 04:04:55 GMT
ENV GOPATH=/go
# Fri, 29 Jul 2016 04:04:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 29 Jul 2016 04:04:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 29 Jul 2016 04:04:58 GMT
WORKDIR /go
# Fri, 29 Jul 2016 04:04:59 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:5c68a10e9f3f9e2757d1f2b0a51ad5ac41f5395a190bbbe3907a6b6fffa9bcea`  
		Last Modified: Thu, 28 Jul 2016 17:54:32 GMT  
		Size: 37.2 MB (37209635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81f9b5104e75c51d678d80525193ab71008b9c25c1a1e4694996b0744c6cbe`  
		Last Modified: Thu, 28 Jul 2016 21:53:17 GMT  
		Size: 6.7 MB (6730996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d9d9752348fab5a9cd1140f31df8ad6ce301aca3e7d4e303d14fde010ea14`  
		Last Modified: Thu, 28 Jul 2016 21:53:49 GMT  
		Size: 38.9 MB (38887392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0238af288e95b46257dcfbe2c650681a0ee6b66bdcf2306ece99f93f1ad794a3`  
		Last Modified: Fri, 29 Jul 2016 03:59:40 GMT  
		Size: 33.9 MB (33949794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453a6a1a4ddc150932047bf9dbfe3b08491372c0de9f889cb58a52e27ea24fbb`  
		Last Modified: Fri, 29 Jul 2016 04:05:37 GMT  
		Size: 84.9 MB (84869331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5ca97ed864658a34e725252086c9b253532062ed97506971694100a94b036e`  
		Last Modified: Fri, 29 Jul 2016 04:05:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b991788ec96628f1f3866f0aab6726922665d5aa247bc8379ca501fc699430c`  
		Last Modified: Fri, 29 Jul 2016 04:05:08 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-alpine`

```console
$ docker pull golang@sha256:8b9e1e4a137e7663c1dc52a33c41699661ea4da9aca6ab0771b1fcec16a87535
```

-	Platforms:
	-	linux; amd64

### `golang:1.6.3-alpine` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72155824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b317e0ae72cec6ec5faa748ae736e1d401735b1dc4eab2c633925ec109b0310`

```dockerfile
# Thu, 23 Jun 2016 19:55:18 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in /
# Fri, 01 Jul 2016 19:29:12 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2016 17:22:23 GMT
ENV GOLANG_VERSION=1.6.3
# Mon, 18 Jul 2016 17:22:24 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.6.3.src.tar.gz
# Mon, 18 Jul 2016 17:22:25 GMT
ENV GOLANG_SRC_SHA256=6326aeed5f86cf18f16d6dc831405614f855e2d416a91fd3fdc334f772345b00
# Mon, 18 Jul 2016 17:22:26 GMT
COPY file:b2d7156cdbff1193fb20efaf40b201017b0396eb5b2e0adb97970615a8fcf61d in /
# Mon, 18 Jul 2016 17:23:41 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Mon, 18 Jul 2016 17:23:42 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2016 17:23:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2016 17:23:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2016 17:23:44 GMT
WORKDIR /go
# Mon, 18 Jul 2016 17:23:44 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac58758e6ad5928c40fe2ce1b955a5f9d1c4889667874887960ff0c00f2ebcf6`  
		Last Modified: Fri, 01 Jul 2016 19:34:13 GMT  
		Size: 343.9 KB (343924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90fc0e5164ab0874b9c887c660857517ef58d35f6506efa6a3c1f086898b99`  
		Last Modified: Mon, 18 Jul 2016 17:30:04 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f38fc389bc155298999428131401648c7470563a4571a304ae564b8cc0ba71`  
		Last Modified: Mon, 18 Jul 2016 17:30:28 GMT  
		Size: 69.5 MB (69499701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087a26f98166190888614f96fb10b95c33c46d1943a6b81a7c66134bd22efa2d`  
		Last Modified: Mon, 18 Jul 2016 17:30:04 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25994cc119744e0d02f5716206b622761006e0fe842624fc0343b68fcbe76804`  
		Last Modified: Mon, 18 Jul 2016 17:30:04 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-alpine`

```console
$ docker pull golang@sha256:8b9e1e4a137e7663c1dc52a33c41699661ea4da9aca6ab0771b1fcec16a87535
```

-	Platforms:
	-	linux; amd64

### `golang:1.6-alpine` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72155824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b317e0ae72cec6ec5faa748ae736e1d401735b1dc4eab2c633925ec109b0310`

```dockerfile
# Thu, 23 Jun 2016 19:55:18 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in /
# Fri, 01 Jul 2016 19:29:12 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2016 17:22:23 GMT
ENV GOLANG_VERSION=1.6.3
# Mon, 18 Jul 2016 17:22:24 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.6.3.src.tar.gz
# Mon, 18 Jul 2016 17:22:25 GMT
ENV GOLANG_SRC_SHA256=6326aeed5f86cf18f16d6dc831405614f855e2d416a91fd3fdc334f772345b00
# Mon, 18 Jul 2016 17:22:26 GMT
COPY file:b2d7156cdbff1193fb20efaf40b201017b0396eb5b2e0adb97970615a8fcf61d in /
# Mon, 18 Jul 2016 17:23:41 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Mon, 18 Jul 2016 17:23:42 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2016 17:23:42 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2016 17:23:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2016 17:23:44 GMT
WORKDIR /go
# Mon, 18 Jul 2016 17:23:44 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac58758e6ad5928c40fe2ce1b955a5f9d1c4889667874887960ff0c00f2ebcf6`  
		Last Modified: Fri, 01 Jul 2016 19:34:13 GMT  
		Size: 343.9 KB (343924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90fc0e5164ab0874b9c887c660857517ef58d35f6506efa6a3c1f086898b99`  
		Last Modified: Mon, 18 Jul 2016 17:30:04 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f38fc389bc155298999428131401648c7470563a4571a304ae564b8cc0ba71`  
		Last Modified: Mon, 18 Jul 2016 17:30:28 GMT  
		Size: 69.5 MB (69499701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087a26f98166190888614f96fb10b95c33c46d1943a6b81a7c66134bd22efa2d`  
		Last Modified: Mon, 18 Jul 2016 17:30:04 GMT  
		Size: 122.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25994cc119744e0d02f5716206b622761006e0fe842624fc0343b68fcbe76804`  
		Last Modified: Mon, 18 Jul 2016 17:30:04 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6.3-windowsservercore`

```console
$ docker pull golang@sha256:c9bab07d3dd2b64f0173fa4e5018097a960b5f9c919a5271eae2418477634a1d
```

-	Platforms:
	-	windows; amd64

### `golang:1.6.3-windowsservercore` - windows; amd64

-	Docker Version: 1.12.0
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 GB (3784047918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27af2ae7b93b6318556028495c550b530cc24d6c6d3bf270e2a010821818a6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 12 Aug 2016 17:01:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 12 Aug 2016 17:01:53 GMT
ENV GIT_VERSION=2.9.2
# Fri, 12 Aug 2016 17:01:58 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Fri, 12 Aug 2016 17:02:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Fri, 12 Aug 2016 17:03:48 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Fri, 12 Aug 2016 23:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GIT_DOWNLOAD_URL, 'git.exe'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:47:34 GMT
ENV GOPATH=C:\gopath
# Fri, 12 Aug 2016 23:47:57 GMT
RUN [Environment]::SetEnvironmentVariable('PATH', $env:GOPATH + '\bin;C:\go\bin;' + $env:PATH, [EnvironmentVariableTarget]::Machine);
# Fri, 12 Aug 2016 23:52:46 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 12 Aug 2016 23:52:49 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.windows-amd64.zip
# Fri, 12 Aug 2016 23:52:52 GMT
ENV GOLANG_DOWNLOAD_SHA256=6a18e5ed8b39785338986aecc6a3f36f5c4be286ff52db0ae3bcd2275ab70df0
# Fri, 12 Aug 2016 23:57:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GOLANG_DOWNLOAD_URL, 'go.zip'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:57:38 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1239394e5a8ab79fbd3b751dc5d98decf5886f14339958fdf5c1f96c89da58a7`  
		Size: 3.5 GB (3461145128 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:be0175dbdd12c150c89a273c6ae8a093858f186a1b130670b81917d39cfc62c3`  
		Last Modified: Tue, 16 Aug 2016 16:11:53 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f7fc8b1eb04be3a8b1a8fc1f9e6c7a1e41689a2676e152c25d9358dee1341`  
		Last Modified: Tue, 16 Aug 2016 16:11:51 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bdc4e8ef7ba6e9f01909b8cb91c6a122e96baef29babe69a01102bcae148c9`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bbfdc9f3a15e9a0bde254b6ab26f6f076cf940ef39c7d7176f7642275bbfda`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b64b13a7ee93c6f86303ad2fe1d9185da583cd6e7ab1671efe67b13e2993a11`  
		Last Modified: Tue, 16 Aug 2016 16:11:37 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e143173cb47f97febd951190e060d115fa15cf474acfb5759c8b410b45a1087`  
		Last Modified: Tue, 16 Aug 2016 16:15:14 GMT  
		Size: 222.7 MB (222712489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de436d4008dda1c26e300dd25d9cc67c8a59a2c0547febbcad41ae4499ea8882`  
		Last Modified: Tue, 16 Aug 2016 16:11:36 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230b17b0e770bf3e266ac0f228d84bf32d942d15e3e5c57d4ec1e5061aa3e51e`  
		Last Modified: Tue, 16 Aug 2016 16:11:42 GMT  
		Size: 4.0 MB (4030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1660cb70ff7044778f5bb23312723c7300a3e00a851ff2b530315747103c7245`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5742033e60baa1364a2cdd957f6061fdaef7abd51cbe5eac8e5414564a7da417`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f57a7d2524daad53adb069be9f9485d038809fc393c83af58a16880787adb`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f9d4477d9e6b931411dad018ac1a0a713c952a8bb51763f44b9c62fd425bab`  
		Last Modified: Tue, 16 Aug 2016 16:16:56 GMT  
		Size: 96.1 MB (96146274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52289dc770d3b6da4f2c1db2cab8052677149d7d86e3f66cdc528a8dfbba467d`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.6-windowsservercore`

```console
$ docker pull golang@sha256:c9bab07d3dd2b64f0173fa4e5018097a960b5f9c919a5271eae2418477634a1d
```

-	Platforms:
	-	windows; amd64

### `golang:1.6-windowsservercore` - windows; amd64

-	Docker Version: 1.12.0
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 GB (3784047918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df27af2ae7b93b6318556028495c550b530cc24d6c6d3bf270e2a010821818a6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 12 Aug 2016 17:01:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 12 Aug 2016 17:01:53 GMT
ENV GIT_VERSION=2.9.2
# Fri, 12 Aug 2016 17:01:58 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Fri, 12 Aug 2016 17:02:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Fri, 12 Aug 2016 17:03:48 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Fri, 12 Aug 2016 23:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GIT_DOWNLOAD_URL, 'git.exe'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:47:34 GMT
ENV GOPATH=C:\gopath
# Fri, 12 Aug 2016 23:47:57 GMT
RUN [Environment]::SetEnvironmentVariable('PATH', $env:GOPATH + '\bin;C:\go\bin;' + $env:PATH, [EnvironmentVariableTarget]::Machine);
# Fri, 12 Aug 2016 23:52:46 GMT
ENV GOLANG_VERSION=1.6.3
# Fri, 12 Aug 2016 23:52:49 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.6.3.windows-amd64.zip
# Fri, 12 Aug 2016 23:52:52 GMT
ENV GOLANG_DOWNLOAD_SHA256=6a18e5ed8b39785338986aecc6a3f36f5c4be286ff52db0ae3bcd2275ab70df0
# Fri, 12 Aug 2016 23:57:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GOLANG_DOWNLOAD_URL, 'go.zip'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:57:38 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1239394e5a8ab79fbd3b751dc5d98decf5886f14339958fdf5c1f96c89da58a7`  
		Size: 3.5 GB (3461145128 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:be0175dbdd12c150c89a273c6ae8a093858f186a1b130670b81917d39cfc62c3`  
		Last Modified: Tue, 16 Aug 2016 16:11:53 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f7fc8b1eb04be3a8b1a8fc1f9e6c7a1e41689a2676e152c25d9358dee1341`  
		Last Modified: Tue, 16 Aug 2016 16:11:51 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bdc4e8ef7ba6e9f01909b8cb91c6a122e96baef29babe69a01102bcae148c9`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bbfdc9f3a15e9a0bde254b6ab26f6f076cf940ef39c7d7176f7642275bbfda`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b64b13a7ee93c6f86303ad2fe1d9185da583cd6e7ab1671efe67b13e2993a11`  
		Last Modified: Tue, 16 Aug 2016 16:11:37 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e143173cb47f97febd951190e060d115fa15cf474acfb5759c8b410b45a1087`  
		Last Modified: Tue, 16 Aug 2016 16:15:14 GMT  
		Size: 222.7 MB (222712489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de436d4008dda1c26e300dd25d9cc67c8a59a2c0547febbcad41ae4499ea8882`  
		Last Modified: Tue, 16 Aug 2016 16:11:36 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230b17b0e770bf3e266ac0f228d84bf32d942d15e3e5c57d4ec1e5061aa3e51e`  
		Last Modified: Tue, 16 Aug 2016 16:11:42 GMT  
		Size: 4.0 MB (4030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1660cb70ff7044778f5bb23312723c7300a3e00a851ff2b530315747103c7245`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5742033e60baa1364a2cdd957f6061fdaef7abd51cbe5eac8e5414564a7da417`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f57a7d2524daad53adb069be9f9485d038809fc393c83af58a16880787adb`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f9d4477d9e6b931411dad018ac1a0a713c952a8bb51763f44b9c62fd425bab`  
		Last Modified: Tue, 16 Aug 2016 16:16:56 GMT  
		Size: 96.1 MB (96146274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52289dc770d3b6da4f2c1db2cab8052677149d7d86e3f66cdc528a8dfbba467d`  
		Last Modified: Tue, 16 Aug 2016 16:15:31 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.0`

```console
$ docker pull golang@sha256:6cdf751b76c8e2c52319941fb189967c1bac3911433871349ac56b82d28e367b
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.0` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe25c00086fbc46741fc62150d197a2f59db658b7f035e0340191079cdbf0baa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7`

```console
$ docker pull golang@sha256:6cdf751b76c8e2c52319941fb189967c1bac3911433871349ac56b82d28e367b
```

-	Platforms:
	-	linux; amd64

### `golang:1.7` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe25c00086fbc46741fc62150d197a2f59db658b7f035e0340191079cdbf0baa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1`

```console
$ docker pull golang@sha256:6cdf751b76c8e2c52319941fb189967c1bac3911433871349ac56b82d28e367b
```

-	Platforms:
	-	linux; amd64

### `golang:1` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe25c00086fbc46741fc62150d197a2f59db658b7f035e0340191079cdbf0baa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:latest`

```console
$ docker pull golang@sha256:6cdf751b76c8e2c52319941fb189967c1bac3911433871349ac56b82d28e367b
```

-	Platforms:
	-	linux; amd64

### `golang:latest` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe25c00086fbc46741fc62150d197a2f59db658b7f035e0340191079cdbf0baa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.0-onbuild`

```console
$ docker pull golang@sha256:28bcf425e686b554e5d1e2651115e85f50aa45ecfdeac5f5f8f579e748cae732
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.0-onbuild` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d20e6703500b53bc61682eb8ee617b69494fb0370b1f51694b31172074579a5`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
# Tue, 16 Aug 2016 17:09:52 GMT
RUN mkdir -p /go/src/app
# Tue, 16 Aug 2016 17:09:53 GMT
WORKDIR /go/src/app
# Tue, 16 Aug 2016 17:09:54 GMT
CMD ["go-wrapper" "run"]
# Tue, 16 Aug 2016 17:09:55 GMT
ONBUILD COPY . /go/src/app
# Tue, 16 Aug 2016 17:10:02 GMT
ONBUILD RUN go-wrapper download
# Tue, 16 Aug 2016 17:10:03 GMT
ONBUILD RUN go-wrapper install
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471e4d355f729ef1819e723e39cace3045b56cf4888246e41bbe71a3fda188c2`  
		Last Modified: Tue, 16 Aug 2016 17:15:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-onbuild`

```console
$ docker pull golang@sha256:28bcf425e686b554e5d1e2651115e85f50aa45ecfdeac5f5f8f579e748cae732
```

-	Platforms:
	-	linux; amd64

### `golang:1.7-onbuild` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d20e6703500b53bc61682eb8ee617b69494fb0370b1f51694b31172074579a5`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
# Tue, 16 Aug 2016 17:09:52 GMT
RUN mkdir -p /go/src/app
# Tue, 16 Aug 2016 17:09:53 GMT
WORKDIR /go/src/app
# Tue, 16 Aug 2016 17:09:54 GMT
CMD ["go-wrapper" "run"]
# Tue, 16 Aug 2016 17:09:55 GMT
ONBUILD COPY . /go/src/app
# Tue, 16 Aug 2016 17:10:02 GMT
ONBUILD RUN go-wrapper download
# Tue, 16 Aug 2016 17:10:03 GMT
ONBUILD RUN go-wrapper install
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471e4d355f729ef1819e723e39cace3045b56cf4888246e41bbe71a3fda188c2`  
		Last Modified: Tue, 16 Aug 2016 17:15:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-onbuild`

```console
$ docker pull golang@sha256:28bcf425e686b554e5d1e2651115e85f50aa45ecfdeac5f5f8f579e748cae732
```

-	Platforms:
	-	linux; amd64

### `golang:1-onbuild` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d20e6703500b53bc61682eb8ee617b69494fb0370b1f51694b31172074579a5`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
# Tue, 16 Aug 2016 17:09:52 GMT
RUN mkdir -p /go/src/app
# Tue, 16 Aug 2016 17:09:53 GMT
WORKDIR /go/src/app
# Tue, 16 Aug 2016 17:09:54 GMT
CMD ["go-wrapper" "run"]
# Tue, 16 Aug 2016 17:09:55 GMT
ONBUILD COPY . /go/src/app
# Tue, 16 Aug 2016 17:10:02 GMT
ONBUILD RUN go-wrapper download
# Tue, 16 Aug 2016 17:10:03 GMT
ONBUILD RUN go-wrapper install
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471e4d355f729ef1819e723e39cace3045b56cf4888246e41bbe71a3fda188c2`  
		Last Modified: Tue, 16 Aug 2016 17:15:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:onbuild`

```console
$ docker pull golang@sha256:28bcf425e686b554e5d1e2651115e85f50aa45ecfdeac5f5f8f579e748cae732
```

-	Platforms:
	-	linux; amd64

### `golang:onbuild` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250878264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d20e6703500b53bc61682eb8ee617b69494fb0370b1f51694b31172074579a5`
-	Default Command: `["go-wrapper","run"]`

```dockerfile
# Thu, 28 Jul 2016 17:47:54 GMT
ADD file:0e0565652aa852f62033d99f84892216020d30f64521ded5e72d4940bc4c9697 in /
# Thu, 28 Jul 2016 17:47:55 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 17:57:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 17:59:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:09:22 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:09:23 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:09:24 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:09:36 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:09:38 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:09:39 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:09:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:09:48 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:09:49 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
# Tue, 16 Aug 2016 17:09:52 GMT
RUN mkdir -p /go/src/app
# Tue, 16 Aug 2016 17:09:53 GMT
WORKDIR /go/src/app
# Tue, 16 Aug 2016 17:09:54 GMT
CMD ["go-wrapper" "run"]
# Tue, 16 Aug 2016 17:09:55 GMT
ONBUILD COPY . /go/src/app
# Tue, 16 Aug 2016 17:10:02 GMT
ONBUILD RUN go-wrapper download
# Tue, 16 Aug 2016 17:10:03 GMT
ONBUILD RUN go-wrapper install
```

-	Layers:
	-	`sha256:357ea8c3d80bc25792e010facfc98aee5972ebc47e290eb0d5aea3671a901cab`  
		Last Modified: Thu, 28 Jul 2016 17:49:58 GMT  
		Size: 51.4 MB (51365611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52befadefd24601247558f63fcb2ccd96b79cbc447a148ea1d0aa2719a9ac3b1`  
		Last Modified: Thu, 28 Jul 2016 21:52:07 GMT  
		Size: 18.5 MB (18526978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0732d5313c8ec8477e518f3e0af81796bdb047ed48cf256333785fc9916ba1`  
		Last Modified: Thu, 28 Jul 2016 21:52:20 GMT  
		Size: 42.5 MB (42495385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee55c62229822bb787bc8502672cac358825b228a0d72ea48b71f6814a92ef4`  
		Last Modified: Fri, 29 Jul 2016 03:56:36 GMT  
		Size: 56.9 MB (56904467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a447620c727235489b4feaf150bbd9f44951c36cdaeee0d927e5daaff3c68`  
		Last Modified: Tue, 16 Aug 2016 17:14:15 GMT  
		Size: 81.6 MB (81584218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eeb61bb0b67b6f3fcf78adbd2408b553818d55cab666a818278efe55ff6db2`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487c6f81373dfd17f84c60a77d8e5ecace3543a6c6b538f83d6e3a008b6f8f9c`  
		Last Modified: Tue, 16 Aug 2016 17:13:50 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471e4d355f729ef1819e723e39cace3045b56cf4888246e41bbe71a3fda188c2`  
		Last Modified: Tue, 16 Aug 2016 17:15:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.0-wheezy`

```console
$ docker pull golang@sha256:79cab6e3c835c081f5a446076f1b448539dcb2d203116041ff0e6e1b8447b337
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.0-wheezy` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198363563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a144f4fe2c464697ab54d43c2c2a731ab5dfb0f8a22a037659785e0d0d267ac7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:49:29 GMT
ADD file:0d2a68d1c5a4a52b0bddd8921fe9f3d603a5d69911d4bba61c5e2460e6500d76 in /
# Thu, 28 Jul 2016 17:49:29 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 18:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 18:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:10:05 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:06 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:10:07 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:10:19 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:10:20 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:10:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:10:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:10:31 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:10:32 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:5c68a10e9f3f9e2757d1f2b0a51ad5ac41f5395a190bbbe3907a6b6fffa9bcea`  
		Last Modified: Thu, 28 Jul 2016 17:54:32 GMT  
		Size: 37.2 MB (37209635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81f9b5104e75c51d678d80525193ab71008b9c25c1a1e4694996b0744c6cbe`  
		Last Modified: Thu, 28 Jul 2016 21:53:17 GMT  
		Size: 6.7 MB (6730996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d9d9752348fab5a9cd1140f31df8ad6ce301aca3e7d4e303d14fde010ea14`  
		Last Modified: Thu, 28 Jul 2016 21:53:49 GMT  
		Size: 38.9 MB (38887392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0238af288e95b46257dcfbe2c650681a0ee6b66bdcf2306ece99f93f1ad794a3`  
		Last Modified: Fri, 29 Jul 2016 03:59:40 GMT  
		Size: 33.9 MB (33949794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766aef40ab5df7cbf2931555beafb9335801643169cb8b5c30ebc931442aad6`  
		Last Modified: Tue, 16 Aug 2016 17:16:24 GMT  
		Size: 81.6 MB (81584267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea8baade0747a902d1c87f81b7c47a5c5d4303aa49ac291d9957b117fc8e59c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187f24b06c1f598955220f8729dbced84fee66d386d2055700d6085f002a363c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-wheezy`

```console
$ docker pull golang@sha256:79cab6e3c835c081f5a446076f1b448539dcb2d203116041ff0e6e1b8447b337
```

-	Platforms:
	-	linux; amd64

### `golang:1.7-wheezy` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198363563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a144f4fe2c464697ab54d43c2c2a731ab5dfb0f8a22a037659785e0d0d267ac7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:49:29 GMT
ADD file:0d2a68d1c5a4a52b0bddd8921fe9f3d603a5d69911d4bba61c5e2460e6500d76 in /
# Thu, 28 Jul 2016 17:49:29 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 18:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 18:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:10:05 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:06 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:10:07 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:10:19 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:10:20 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:10:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:10:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:10:31 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:10:32 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:5c68a10e9f3f9e2757d1f2b0a51ad5ac41f5395a190bbbe3907a6b6fffa9bcea`  
		Last Modified: Thu, 28 Jul 2016 17:54:32 GMT  
		Size: 37.2 MB (37209635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81f9b5104e75c51d678d80525193ab71008b9c25c1a1e4694996b0744c6cbe`  
		Last Modified: Thu, 28 Jul 2016 21:53:17 GMT  
		Size: 6.7 MB (6730996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d9d9752348fab5a9cd1140f31df8ad6ce301aca3e7d4e303d14fde010ea14`  
		Last Modified: Thu, 28 Jul 2016 21:53:49 GMT  
		Size: 38.9 MB (38887392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0238af288e95b46257dcfbe2c650681a0ee6b66bdcf2306ece99f93f1ad794a3`  
		Last Modified: Fri, 29 Jul 2016 03:59:40 GMT  
		Size: 33.9 MB (33949794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766aef40ab5df7cbf2931555beafb9335801643169cb8b5c30ebc931442aad6`  
		Last Modified: Tue, 16 Aug 2016 17:16:24 GMT  
		Size: 81.6 MB (81584267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea8baade0747a902d1c87f81b7c47a5c5d4303aa49ac291d9957b117fc8e59c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187f24b06c1f598955220f8729dbced84fee66d386d2055700d6085f002a363c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-wheezy`

```console
$ docker pull golang@sha256:79cab6e3c835c081f5a446076f1b448539dcb2d203116041ff0e6e1b8447b337
```

-	Platforms:
	-	linux; amd64

### `golang:1-wheezy` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198363563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a144f4fe2c464697ab54d43c2c2a731ab5dfb0f8a22a037659785e0d0d267ac7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:49:29 GMT
ADD file:0d2a68d1c5a4a52b0bddd8921fe9f3d603a5d69911d4bba61c5e2460e6500d76 in /
# Thu, 28 Jul 2016 17:49:29 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 18:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 18:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:10:05 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:06 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:10:07 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:10:19 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:10:20 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:10:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:10:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:10:31 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:10:32 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:5c68a10e9f3f9e2757d1f2b0a51ad5ac41f5395a190bbbe3907a6b6fffa9bcea`  
		Last Modified: Thu, 28 Jul 2016 17:54:32 GMT  
		Size: 37.2 MB (37209635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81f9b5104e75c51d678d80525193ab71008b9c25c1a1e4694996b0744c6cbe`  
		Last Modified: Thu, 28 Jul 2016 21:53:17 GMT  
		Size: 6.7 MB (6730996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d9d9752348fab5a9cd1140f31df8ad6ce301aca3e7d4e303d14fde010ea14`  
		Last Modified: Thu, 28 Jul 2016 21:53:49 GMT  
		Size: 38.9 MB (38887392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0238af288e95b46257dcfbe2c650681a0ee6b66bdcf2306ece99f93f1ad794a3`  
		Last Modified: Fri, 29 Jul 2016 03:59:40 GMT  
		Size: 33.9 MB (33949794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766aef40ab5df7cbf2931555beafb9335801643169cb8b5c30ebc931442aad6`  
		Last Modified: Tue, 16 Aug 2016 17:16:24 GMT  
		Size: 81.6 MB (81584267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea8baade0747a902d1c87f81b7c47a5c5d4303aa49ac291d9957b117fc8e59c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187f24b06c1f598955220f8729dbced84fee66d386d2055700d6085f002a363c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:wheezy`

```console
$ docker pull golang@sha256:79cab6e3c835c081f5a446076f1b448539dcb2d203116041ff0e6e1b8447b337
```

-	Platforms:
	-	linux; amd64

### `golang:wheezy` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198363563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a144f4fe2c464697ab54d43c2c2a731ab5dfb0f8a22a037659785e0d0d267ac7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 28 Jul 2016 17:49:29 GMT
ADD file:0d2a68d1c5a4a52b0bddd8921fe9f3d603a5d69911d4bba61c5e2460e6500d76 in /
# Thu, 28 Jul 2016 17:49:29 GMT
CMD ["/bin/bash"]
# Thu, 28 Jul 2016 18:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2016 18:28:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2016 03:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		g++ 		gcc 		libc6-dev 		make 	&& rm -rf /var/lib/apt/lists/*
# Tue, 16 Aug 2016 17:10:05 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:06 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.linux-amd64.tar.gz
# Tue, 16 Aug 2016 17:10:07 GMT
ENV GOLANG_DOWNLOAD_SHA256=702ad90f705365227e902b42d91dd1a40e48ca7f67a2f4b2fd052aaa4295cd95
# Tue, 16 Aug 2016 17:10:19 GMT
RUN curl -fsSL "$GOLANG_DOWNLOAD_URL" -o golang.tar.gz 	&& echo "$GOLANG_DOWNLOAD_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz
# Tue, 16 Aug 2016 17:10:20 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:10:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:10:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:10:31 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:10:32 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:5c68a10e9f3f9e2757d1f2b0a51ad5ac41f5395a190bbbe3907a6b6fffa9bcea`  
		Last Modified: Thu, 28 Jul 2016 17:54:32 GMT  
		Size: 37.2 MB (37209635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c81f9b5104e75c51d678d80525193ab71008b9c25c1a1e4694996b0744c6cbe`  
		Last Modified: Thu, 28 Jul 2016 21:53:17 GMT  
		Size: 6.7 MB (6730996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d9d9752348fab5a9cd1140f31df8ad6ce301aca3e7d4e303d14fde010ea14`  
		Last Modified: Thu, 28 Jul 2016 21:53:49 GMT  
		Size: 38.9 MB (38887392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0238af288e95b46257dcfbe2c650681a0ee6b66bdcf2306ece99f93f1ad794a3`  
		Last Modified: Fri, 29 Jul 2016 03:59:40 GMT  
		Size: 33.9 MB (33949794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5766aef40ab5df7cbf2931555beafb9335801643169cb8b5c30ebc931442aad6`  
		Last Modified: Tue, 16 Aug 2016 17:16:24 GMT  
		Size: 81.6 MB (81584267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea8baade0747a902d1c87f81b7c47a5c5d4303aa49ac291d9957b117fc8e59c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187f24b06c1f598955220f8729dbced84fee66d386d2055700d6085f002a363c`  
		Last Modified: Tue, 16 Aug 2016 17:15:58 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.0-alpine`

```console
$ docker pull golang@sha256:e91d55a5eaf99dcd05391094cb33a33e728384d9d05673e6749584246ea79206
```

-	Platforms:
	-	linux; amd64

### `golang:1.7.0-alpine` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73263041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52493611af1ebc424812b8ad8029b2c6c53b4d0551052e65c985efefcd688547`

```dockerfile
# Thu, 23 Jun 2016 19:55:18 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in /
# Fri, 01 Jul 2016 19:29:12 GMT
RUN apk add --no-cache ca-certificates
# Tue, 16 Aug 2016 17:10:34 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:35 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.src.tar.gz
# Tue, 16 Aug 2016 17:10:36 GMT
ENV GOLANG_SRC_SHA256=72680c16ba0891fcf2ccf46d0f809e4ecf47bbf889f5d884ccb54c5e9a17e1c0
# Tue, 16 Aug 2016 17:10:37 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in /
# Tue, 16 Aug 2016 17:12:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Tue, 16 Aug 2016 17:12:02 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:12:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:12:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:12:07 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:12:08 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac58758e6ad5928c40fe2ce1b955a5f9d1c4889667874887960ff0c00f2ebcf6`  
		Last Modified: Fri, 01 Jul 2016 19:34:13 GMT  
		Size: 343.9 KB (343924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d730108ef4ddf04d261f18ee59590e84c4f72c59e25df6d45747d7443af9bc64`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9a517a6ac1e571d5f5a872aa5a1fd0d202dd711f51fcaa778f407c8206152`  
		Last Modified: Tue, 16 Aug 2016 17:17:39 GMT  
		Size: 70.6 MB (70606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d02ce012bc58b5a8d75993625cd8ffc7945c3bf2bdcde128a471369008e33`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca6005cc852f36060697fbcc205308c24eaf2b2d03dd0743f258bc4ba34dc6`  
		Last Modified: Tue, 16 Aug 2016 17:17:15 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-alpine`

```console
$ docker pull golang@sha256:e91d55a5eaf99dcd05391094cb33a33e728384d9d05673e6749584246ea79206
```

-	Platforms:
	-	linux; amd64

### `golang:1.7-alpine` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73263041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52493611af1ebc424812b8ad8029b2c6c53b4d0551052e65c985efefcd688547`

```dockerfile
# Thu, 23 Jun 2016 19:55:18 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in /
# Fri, 01 Jul 2016 19:29:12 GMT
RUN apk add --no-cache ca-certificates
# Tue, 16 Aug 2016 17:10:34 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:35 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.src.tar.gz
# Tue, 16 Aug 2016 17:10:36 GMT
ENV GOLANG_SRC_SHA256=72680c16ba0891fcf2ccf46d0f809e4ecf47bbf889f5d884ccb54c5e9a17e1c0
# Tue, 16 Aug 2016 17:10:37 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in /
# Tue, 16 Aug 2016 17:12:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Tue, 16 Aug 2016 17:12:02 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:12:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:12:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:12:07 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:12:08 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac58758e6ad5928c40fe2ce1b955a5f9d1c4889667874887960ff0c00f2ebcf6`  
		Last Modified: Fri, 01 Jul 2016 19:34:13 GMT  
		Size: 343.9 KB (343924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d730108ef4ddf04d261f18ee59590e84c4f72c59e25df6d45747d7443af9bc64`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9a517a6ac1e571d5f5a872aa5a1fd0d202dd711f51fcaa778f407c8206152`  
		Last Modified: Tue, 16 Aug 2016 17:17:39 GMT  
		Size: 70.6 MB (70606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d02ce012bc58b5a8d75993625cd8ffc7945c3bf2bdcde128a471369008e33`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca6005cc852f36060697fbcc205308c24eaf2b2d03dd0743f258bc4ba34dc6`  
		Last Modified: Tue, 16 Aug 2016 17:17:15 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-alpine`

```console
$ docker pull golang@sha256:e91d55a5eaf99dcd05391094cb33a33e728384d9d05673e6749584246ea79206
```

-	Platforms:
	-	linux; amd64

### `golang:1-alpine` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73263041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52493611af1ebc424812b8ad8029b2c6c53b4d0551052e65c985efefcd688547`

```dockerfile
# Thu, 23 Jun 2016 19:55:18 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in /
# Fri, 01 Jul 2016 19:29:12 GMT
RUN apk add --no-cache ca-certificates
# Tue, 16 Aug 2016 17:10:34 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:35 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.src.tar.gz
# Tue, 16 Aug 2016 17:10:36 GMT
ENV GOLANG_SRC_SHA256=72680c16ba0891fcf2ccf46d0f809e4ecf47bbf889f5d884ccb54c5e9a17e1c0
# Tue, 16 Aug 2016 17:10:37 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in /
# Tue, 16 Aug 2016 17:12:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Tue, 16 Aug 2016 17:12:02 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:12:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:12:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:12:07 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:12:08 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac58758e6ad5928c40fe2ce1b955a5f9d1c4889667874887960ff0c00f2ebcf6`  
		Last Modified: Fri, 01 Jul 2016 19:34:13 GMT  
		Size: 343.9 KB (343924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d730108ef4ddf04d261f18ee59590e84c4f72c59e25df6d45747d7443af9bc64`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9a517a6ac1e571d5f5a872aa5a1fd0d202dd711f51fcaa778f407c8206152`  
		Last Modified: Tue, 16 Aug 2016 17:17:39 GMT  
		Size: 70.6 MB (70606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d02ce012bc58b5a8d75993625cd8ffc7945c3bf2bdcde128a471369008e33`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca6005cc852f36060697fbcc205308c24eaf2b2d03dd0743f258bc4ba34dc6`  
		Last Modified: Tue, 16 Aug 2016 17:17:15 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:alpine`

```console
$ docker pull golang@sha256:e91d55a5eaf99dcd05391094cb33a33e728384d9d05673e6749584246ea79206
```

-	Platforms:
	-	linux; amd64

### `golang:alpine` - linux; amd64

-	Docker Version: 1.10.3
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73263041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52493611af1ebc424812b8ad8029b2c6c53b4d0551052e65c985efefcd688547`

```dockerfile
# Thu, 23 Jun 2016 19:55:18 GMT
ADD file:852e9d0cb9d906535af512a89339fc70b2873a0f94defbcbe41cd44942dd6ac8 in /
# Fri, 01 Jul 2016 19:29:12 GMT
RUN apk add --no-cache ca-certificates
# Tue, 16 Aug 2016 17:10:34 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 17:10:35 GMT
ENV GOLANG_SRC_URL=https://golang.org/dl/go1.7.src.tar.gz
# Tue, 16 Aug 2016 17:10:36 GMT
ENV GOLANG_SRC_SHA256=72680c16ba0891fcf2ccf46d0f809e4ecf47bbf889f5d884ccb54c5e9a17e1c0
# Tue, 16 Aug 2016 17:10:37 GMT
COPY file:b54d7d4313a41e3729d6f4b7aa6e6f33a1e99759cb2a04149fae89f8211c3a65 in /
# Tue, 16 Aug 2016 17:12:01 GMT
RUN set -ex 	&& apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 		&& export GOROOT_BOOTSTRAP="$(go env GOROOT)" 		&& wget -q "$GOLANG_SRC_URL" -O golang.tar.gz 	&& echo "$GOLANG_SRC_SHA256  golang.tar.gz" | sha256sum -c - 	&& tar -C /usr/local -xzf golang.tar.gz 	&& rm golang.tar.gz 	&& cd /usr/local/go/src 	&& patch -p2 -i /no-pic.patch 	&& ./make.bash 		&& rm -rf /*.patch 	&& apk del .build-deps
# Tue, 16 Aug 2016 17:12:02 GMT
ENV GOPATH=/go
# Tue, 16 Aug 2016 17:12:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 16 Aug 2016 17:12:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 16 Aug 2016 17:12:07 GMT
WORKDIR /go
# Tue, 16 Aug 2016 17:12:08 GMT
COPY file:f6191f2c86edc9343569339f101facba47e886e33e29d70da6916ca6b1101a53 in /usr/local/bin/
```

-	Layers:
	-	`sha256:e110a4a1794126ef308a49f2d65785af2f25538f06700721aad8283b81fdfa58`  
		Last Modified: Thu, 23 Jun 2016 19:56:16 GMT  
		Size: 2.3 MB (2310286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac58758e6ad5928c40fe2ce1b955a5f9d1c4889667874887960ff0c00f2ebcf6`  
		Last Modified: Fri, 01 Jul 2016 19:34:13 GMT  
		Size: 343.9 KB (343924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d730108ef4ddf04d261f18ee59590e84c4f72c59e25df6d45747d7443af9bc64`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9a517a6ac1e571d5f5a872aa5a1fd0d202dd711f51fcaa778f407c8206152`  
		Last Modified: Tue, 16 Aug 2016 17:17:39 GMT  
		Size: 70.6 MB (70606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d02ce012bc58b5a8d75993625cd8ffc7945c3bf2bdcde128a471369008e33`  
		Last Modified: Tue, 16 Aug 2016 17:17:16 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca6005cc852f36060697fbcc205308c24eaf2b2d03dd0743f258bc4ba34dc6`  
		Last Modified: Tue, 16 Aug 2016 17:17:15 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7.0-windowsservercore`

```console
$ docker pull golang@sha256:36366df33f506c7f05d933cdb729e3432d026e02c7fa0d94a936cb945ef09230
```

-	Platforms:
	-	windows; amd64

### `golang:1.7.0-windowsservercore` - windows; amd64

-	Docker Version: 1.12.0
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 GB (3781087656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633190b5643a34196b3b2800c48593e3a32fda2d408af8130cb0d99dfc542574`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 12 Aug 2016 17:01:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 12 Aug 2016 17:01:53 GMT
ENV GIT_VERSION=2.9.2
# Fri, 12 Aug 2016 17:01:58 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Fri, 12 Aug 2016 17:02:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Fri, 12 Aug 2016 17:03:48 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Fri, 12 Aug 2016 23:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GIT_DOWNLOAD_URL, 'git.exe'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:47:34 GMT
ENV GOPATH=C:\gopath
# Fri, 12 Aug 2016 23:47:57 GMT
RUN [Environment]::SetEnvironmentVariable('PATH', $env:GOPATH + '\bin;C:\go\bin;' + $env:PATH, [EnvironmentVariableTarget]::Machine);
# Tue, 16 Aug 2016 00:03:27 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 16:43:40 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.windows-amd64.zip
# Tue, 16 Aug 2016 16:43:44 GMT
ENV GOLANG_DOWNLOAD_SHA256=f51aad06644cc8bd119d2f6933334fa8da24d26e6676fde022cecf5978f1a0c7
# Tue, 16 Aug 2016 16:49:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GOLANG_DOWNLOAD_URL, 'go.zip'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 16 Aug 2016 16:49:07 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1239394e5a8ab79fbd3b751dc5d98decf5886f14339958fdf5c1f96c89da58a7`  
		Size: 3.5 GB (3461145128 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:be0175dbdd12c150c89a273c6ae8a093858f186a1b130670b81917d39cfc62c3`  
		Last Modified: Tue, 16 Aug 2016 16:11:53 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f7fc8b1eb04be3a8b1a8fc1f9e6c7a1e41689a2676e152c25d9358dee1341`  
		Last Modified: Tue, 16 Aug 2016 16:11:51 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bdc4e8ef7ba6e9f01909b8cb91c6a122e96baef29babe69a01102bcae148c9`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bbfdc9f3a15e9a0bde254b6ab26f6f076cf940ef39c7d7176f7642275bbfda`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b64b13a7ee93c6f86303ad2fe1d9185da583cd6e7ab1671efe67b13e2993a11`  
		Last Modified: Tue, 16 Aug 2016 16:11:37 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e143173cb47f97febd951190e060d115fa15cf474acfb5759c8b410b45a1087`  
		Last Modified: Tue, 16 Aug 2016 16:15:14 GMT  
		Size: 222.7 MB (222712489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de436d4008dda1c26e300dd25d9cc67c8a59a2c0547febbcad41ae4499ea8882`  
		Last Modified: Tue, 16 Aug 2016 16:11:36 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230b17b0e770bf3e266ac0f228d84bf32d942d15e3e5c57d4ec1e5061aa3e51e`  
		Last Modified: Tue, 16 Aug 2016 16:11:42 GMT  
		Size: 4.0 MB (4030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447de67ea2419aa2f8028e0fddf31710545f9ee8c9c813e1888f219a6614959`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bbaa533ba7033fdaacd5a996517393d2c8220f7965dcbd6658800f6d1b75fe`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b47bb2bb68a606c91182bcd7724b7723f48341d6c24256e75c9b9d3a57b3f8`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835a8eeea92e980cb5e8a4deddb8dc46d36795c13a7aa2ff3a9c22a91e5c95d`  
		Last Modified: Tue, 16 Aug 2016 17:10:00 GMT  
		Size: 93.2 MB (93186010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4af9de300cbd6f3f16e1daa9512a23f54638eb19f1db4a6f2da293febc25dea`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1.7-windowsservercore`

```console
$ docker pull golang@sha256:36366df33f506c7f05d933cdb729e3432d026e02c7fa0d94a936cb945ef09230
```

-	Platforms:
	-	windows; amd64

### `golang:1.7-windowsservercore` - windows; amd64

-	Docker Version: 1.12.0
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 GB (3781087656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633190b5643a34196b3b2800c48593e3a32fda2d408af8130cb0d99dfc542574`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 12 Aug 2016 17:01:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 12 Aug 2016 17:01:53 GMT
ENV GIT_VERSION=2.9.2
# Fri, 12 Aug 2016 17:01:58 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Fri, 12 Aug 2016 17:02:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Fri, 12 Aug 2016 17:03:48 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Fri, 12 Aug 2016 23:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GIT_DOWNLOAD_URL, 'git.exe'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:47:34 GMT
ENV GOPATH=C:\gopath
# Fri, 12 Aug 2016 23:47:57 GMT
RUN [Environment]::SetEnvironmentVariable('PATH', $env:GOPATH + '\bin;C:\go\bin;' + $env:PATH, [EnvironmentVariableTarget]::Machine);
# Tue, 16 Aug 2016 00:03:27 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 16:43:40 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.windows-amd64.zip
# Tue, 16 Aug 2016 16:43:44 GMT
ENV GOLANG_DOWNLOAD_SHA256=f51aad06644cc8bd119d2f6933334fa8da24d26e6676fde022cecf5978f1a0c7
# Tue, 16 Aug 2016 16:49:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GOLANG_DOWNLOAD_URL, 'go.zip'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 16 Aug 2016 16:49:07 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1239394e5a8ab79fbd3b751dc5d98decf5886f14339958fdf5c1f96c89da58a7`  
		Size: 3.5 GB (3461145128 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:be0175dbdd12c150c89a273c6ae8a093858f186a1b130670b81917d39cfc62c3`  
		Last Modified: Tue, 16 Aug 2016 16:11:53 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f7fc8b1eb04be3a8b1a8fc1f9e6c7a1e41689a2676e152c25d9358dee1341`  
		Last Modified: Tue, 16 Aug 2016 16:11:51 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bdc4e8ef7ba6e9f01909b8cb91c6a122e96baef29babe69a01102bcae148c9`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bbfdc9f3a15e9a0bde254b6ab26f6f076cf940ef39c7d7176f7642275bbfda`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b64b13a7ee93c6f86303ad2fe1d9185da583cd6e7ab1671efe67b13e2993a11`  
		Last Modified: Tue, 16 Aug 2016 16:11:37 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e143173cb47f97febd951190e060d115fa15cf474acfb5759c8b410b45a1087`  
		Last Modified: Tue, 16 Aug 2016 16:15:14 GMT  
		Size: 222.7 MB (222712489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de436d4008dda1c26e300dd25d9cc67c8a59a2c0547febbcad41ae4499ea8882`  
		Last Modified: Tue, 16 Aug 2016 16:11:36 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230b17b0e770bf3e266ac0f228d84bf32d942d15e3e5c57d4ec1e5061aa3e51e`  
		Last Modified: Tue, 16 Aug 2016 16:11:42 GMT  
		Size: 4.0 MB (4030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447de67ea2419aa2f8028e0fddf31710545f9ee8c9c813e1888f219a6614959`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bbaa533ba7033fdaacd5a996517393d2c8220f7965dcbd6658800f6d1b75fe`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b47bb2bb68a606c91182bcd7724b7723f48341d6c24256e75c9b9d3a57b3f8`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835a8eeea92e980cb5e8a4deddb8dc46d36795c13a7aa2ff3a9c22a91e5c95d`  
		Last Modified: Tue, 16 Aug 2016 17:10:00 GMT  
		Size: 93.2 MB (93186010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4af9de300cbd6f3f16e1daa9512a23f54638eb19f1db4a6f2da293febc25dea`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:1-windowsservercore`

```console
$ docker pull golang@sha256:36366df33f506c7f05d933cdb729e3432d026e02c7fa0d94a936cb945ef09230
```

-	Platforms:
	-	windows; amd64

### `golang:1-windowsservercore` - windows; amd64

-	Docker Version: 1.12.0
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 GB (3781087656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633190b5643a34196b3b2800c48593e3a32fda2d408af8130cb0d99dfc542574`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 12 Aug 2016 17:01:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 12 Aug 2016 17:01:53 GMT
ENV GIT_VERSION=2.9.2
# Fri, 12 Aug 2016 17:01:58 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Fri, 12 Aug 2016 17:02:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Fri, 12 Aug 2016 17:03:48 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Fri, 12 Aug 2016 23:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GIT_DOWNLOAD_URL, 'git.exe'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:47:34 GMT
ENV GOPATH=C:\gopath
# Fri, 12 Aug 2016 23:47:57 GMT
RUN [Environment]::SetEnvironmentVariable('PATH', $env:GOPATH + '\bin;C:\go\bin;' + $env:PATH, [EnvironmentVariableTarget]::Machine);
# Tue, 16 Aug 2016 00:03:27 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 16:43:40 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.windows-amd64.zip
# Tue, 16 Aug 2016 16:43:44 GMT
ENV GOLANG_DOWNLOAD_SHA256=f51aad06644cc8bd119d2f6933334fa8da24d26e6676fde022cecf5978f1a0c7
# Tue, 16 Aug 2016 16:49:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GOLANG_DOWNLOAD_URL, 'go.zip'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 16 Aug 2016 16:49:07 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1239394e5a8ab79fbd3b751dc5d98decf5886f14339958fdf5c1f96c89da58a7`  
		Size: 3.5 GB (3461145128 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:be0175dbdd12c150c89a273c6ae8a093858f186a1b130670b81917d39cfc62c3`  
		Last Modified: Tue, 16 Aug 2016 16:11:53 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f7fc8b1eb04be3a8b1a8fc1f9e6c7a1e41689a2676e152c25d9358dee1341`  
		Last Modified: Tue, 16 Aug 2016 16:11:51 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bdc4e8ef7ba6e9f01909b8cb91c6a122e96baef29babe69a01102bcae148c9`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bbfdc9f3a15e9a0bde254b6ab26f6f076cf940ef39c7d7176f7642275bbfda`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b64b13a7ee93c6f86303ad2fe1d9185da583cd6e7ab1671efe67b13e2993a11`  
		Last Modified: Tue, 16 Aug 2016 16:11:37 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e143173cb47f97febd951190e060d115fa15cf474acfb5759c8b410b45a1087`  
		Last Modified: Tue, 16 Aug 2016 16:15:14 GMT  
		Size: 222.7 MB (222712489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de436d4008dda1c26e300dd25d9cc67c8a59a2c0547febbcad41ae4499ea8882`  
		Last Modified: Tue, 16 Aug 2016 16:11:36 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230b17b0e770bf3e266ac0f228d84bf32d942d15e3e5c57d4ec1e5061aa3e51e`  
		Last Modified: Tue, 16 Aug 2016 16:11:42 GMT  
		Size: 4.0 MB (4030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447de67ea2419aa2f8028e0fddf31710545f9ee8c9c813e1888f219a6614959`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bbaa533ba7033fdaacd5a996517393d2c8220f7965dcbd6658800f6d1b75fe`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b47bb2bb68a606c91182bcd7724b7723f48341d6c24256e75c9b9d3a57b3f8`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835a8eeea92e980cb5e8a4deddb8dc46d36795c13a7aa2ff3a9c22a91e5c95d`  
		Last Modified: Tue, 16 Aug 2016 17:10:00 GMT  
		Size: 93.2 MB (93186010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4af9de300cbd6f3f16e1daa9512a23f54638eb19f1db4a6f2da293febc25dea`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `golang:windowsservercore`

```console
$ docker pull golang@sha256:36366df33f506c7f05d933cdb729e3432d026e02c7fa0d94a936cb945ef09230
```

-	Platforms:
	-	windows; amd64

### `golang:windowsservercore` - windows; amd64

-	Docker Version: 1.12.0
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 GB (3781087656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:633190b5643a34196b3b2800c48593e3a32fda2d408af8130cb0d99dfc542574`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 12 Aug 2016 17:01:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 12 Aug 2016 17:01:53 GMT
ENV GIT_VERSION=2.9.2
# Fri, 12 Aug 2016 17:01:58 GMT
ENV GIT_TAG=v2.9.2.windows.1
# Fri, 12 Aug 2016 17:02:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.9.2.windows.1/Git-2.9.2-64-bit.exe
# Fri, 12 Aug 2016 17:03:48 GMT
ENV GIT_DOWNLOAD_SHA256=006d971bcbe73cc8d841a100a4eb20d22e135142bf5b0f2120722fd420e166e5
# Fri, 12 Aug 2016 23:47:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GIT_DOWNLOAD_URL, 'git.exe'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.exe -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-Wait 		-FilePath ./git.exe 		-ArgumentList @( 			'/VERYSILENT', 			'/NORESTART', 			'/NOCANCEL', 			'/SP-', 			'/SUPPRESSMSGBOXES', 						'/COMPONENTS=assoc_sh', 						'/DIR=C:\git' 		); 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\bin;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 	Write-Host '  bash --version'; bash --version; 	Write-Host '  curl --version'; curl.exe --version; 		Write-Host 'Removing installer ...'; 	Remove-Item git.exe -Force; 		Write-Host 'Complete.';
# Fri, 12 Aug 2016 23:47:34 GMT
ENV GOPATH=C:\gopath
# Fri, 12 Aug 2016 23:47:57 GMT
RUN [Environment]::SetEnvironmentVariable('PATH', $env:GOPATH + '\bin;C:\go\bin;' + $env:PATH, [EnvironmentVariableTarget]::Machine);
# Tue, 16 Aug 2016 00:03:27 GMT
ENV GOLANG_VERSION=1.7
# Tue, 16 Aug 2016 16:43:40 GMT
ENV GOLANG_DOWNLOAD_URL=https://golang.org/dl/go1.7.windows-amd64.zip
# Tue, 16 Aug 2016 16:43:44 GMT
ENV GOLANG_DOWNLOAD_SHA256=f51aad06644cc8bd119d2f6933334fa8da24d26e6676fde022cecf5978f1a0c7
# Tue, 16 Aug 2016 16:49:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GOLANG_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:GOLANG_DOWNLOAD_URL, 'go.zip'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GOLANG_DOWNLOAD_SHA256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $env:GOLANG_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Tue, 16 Aug 2016 16:49:07 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:1239394e5a8ab79fbd3b751dc5d98decf5886f14339958fdf5c1f96c89da58a7`  
		Size: 3.5 GB (3461145128 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:be0175dbdd12c150c89a273c6ae8a093858f186a1b130670b81917d39cfc62c3`  
		Last Modified: Tue, 16 Aug 2016 16:11:53 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a9f7fc8b1eb04be3a8b1a8fc1f9e6c7a1e41689a2676e152c25d9358dee1341`  
		Last Modified: Tue, 16 Aug 2016 16:11:51 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bdc4e8ef7ba6e9f01909b8cb91c6a122e96baef29babe69a01102bcae148c9`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bbfdc9f3a15e9a0bde254b6ab26f6f076cf940ef39c7d7176f7642275bbfda`  
		Last Modified: Tue, 16 Aug 2016 16:11:47 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b64b13a7ee93c6f86303ad2fe1d9185da583cd6e7ab1671efe67b13e2993a11`  
		Last Modified: Tue, 16 Aug 2016 16:11:37 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e143173cb47f97febd951190e060d115fa15cf474acfb5759c8b410b45a1087`  
		Last Modified: Tue, 16 Aug 2016 16:15:14 GMT  
		Size: 222.7 MB (222712489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de436d4008dda1c26e300dd25d9cc67c8a59a2c0547febbcad41ae4499ea8882`  
		Last Modified: Tue, 16 Aug 2016 16:11:36 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230b17b0e770bf3e266ac0f228d84bf32d942d15e3e5c57d4ec1e5061aa3e51e`  
		Last Modified: Tue, 16 Aug 2016 16:11:42 GMT  
		Size: 4.0 MB (4030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447de67ea2419aa2f8028e0fddf31710545f9ee8c9c813e1888f219a6614959`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bbaa533ba7033fdaacd5a996517393d2c8220f7965dcbd6658800f6d1b75fe`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b47bb2bb68a606c91182bcd7724b7723f48341d6c24256e75c9b9d3a57b3f8`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8835a8eeea92e980cb5e8a4deddb8dc46d36795c13a7aa2ff3a9c22a91e5c95d`  
		Last Modified: Tue, 16 Aug 2016 17:10:00 GMT  
		Size: 93.2 MB (93186010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4af9de300cbd6f3f16e1daa9512a23f54638eb19f1db4a6f2da293febc25dea`  
		Last Modified: Tue, 16 Aug 2016 17:09:11 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
