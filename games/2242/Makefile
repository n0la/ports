# $OpenBSD: Makefile.template,v 1.76 2017/02/25 16:04:20 danj Exp $

COMMENT =	framework and IRC bot for the cyberpunk game 2242

V =		0.0.20171208.0
DISTNAME =	2242-${V}

GH_ACCOUNT =	n0la
GH_PROJECT =	2242
GH_COMMIT =	7c4ce2c05261f405071a08898c9d2a3e5d97e50d

SHARED_LIBS =	qstar		0.0	# 0.0

CATEGORIES =	games

MAINTAINER =		Florian Stinglmayr <florian@n0la.org>

# BSD
PERMIT_PACKAGE_CDROM =	Yes

# If pledge is used, annotate with `uses pledge()' in a comment

WANTLIB =		c

MODULES =		devel/cmake
BUILD_DEPENDS =		devel/glib2 \
			devel/bison \
			net/ibd

.include <bsd.port.mk>
