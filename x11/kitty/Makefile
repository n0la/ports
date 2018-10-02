# $OpenBSD: Makefile.template,v 1.78 2018/07/09 15:00:06 jca Exp $

COMMENT =	fast, feature full, GPU based terminal emulator

V =	0.12.2
DISTNAME =	kitty-${V}

CATEGORIES =	x11

MAINTAINER =		Florian Stinglmayr <florian@n0la.org>

#GPLv3
PERMIT_PACKAGE_CDROM =	Yes

WANTLIB +=	GL X11 X11-xcb Xcursor Xinerama Xrandr c fontconfig \
		freetype intl m pthread util xcb z

MASTER_SITES =		https://github.com/kovidgoyal/kitty/releases/download/v${V}/

EXTRACT_SUFX =		.tar.xz

MODULES =		lang/python
RUN_DEPENDS =		devel/desktop-file-utils \
			x11/gtk+3,-guic

MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}

do-build:

# target `linux-package` is build & install in one
do-install:
	cd ${WRKSRC} && env OVERRIDE_CFLAGS="-Wall -std=gnu99" \
		CC=gcc LD=gcc \
		python3 setup.py linux-package --prefix=${WRKINST}/usr/local

.include <bsd.port.mk>
