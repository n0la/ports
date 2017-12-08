# $OpenBSD: Makefile.template,v 1.76 2017/02/25 16:04:20 danj Exp $

COMMENT =	shitty IRC bot framework

# Once 0.1 is released it will be automatically bigger than 0.0.XXXXX
V =		0.0.20171208.3
DISTNAME =	ibd-${V}

GH_ACCOUNT =	n0la
GH_PROJECT =	ibd
GH_COMMIT = 	52db036ea54aece17d953894737229fc6040a2a9

SHARED_LIBS =	irc		0.0 # 0.1

CATEGORIES =	net

MAINTAINER =		Florian Stinglmayr <florian@n0la.org>

# BSD
PERMIT_PACKAGE_CDROM =	Yes

# If pledge is used, annotate with `uses pledge()' in a comment

WANTLIB =		c crypto pthread ssl tls

MODULES =		devel/cmake
BUILD_DEPENDS =		devel/libevent2 \
			devel/check \
			devel/bison

.include <bsd.port.mk>
