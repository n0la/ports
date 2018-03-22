# $OpenBSD: Makefile.template,v 1.76 2017/02/25 16:04:20 danj Exp $

COMMENT =	console browser for Reddit

V =		1.21.0
DISTNAME =	rtv
PKGNAME =	rtv-${V}

GH_ACCOUNT =	michael-lazar
GH_PROJECT =	rtv
GH_TAGNAME =	v${V}

CATEGORIES =	net

HOMEPAGE =	https://github.com/michael-lazar/rtv

MAINTAINER =		Florian Stinglmayr <florian@n0la.org>

# MIT
PERMIT_PACKAGE_CDROM =	Yes

MODULES =		lang/python
MODPY_VERSION =		${MODPY_DEFAULT_VERSION_3}
MODPY_SETUPTOOLS =	Yes
RUN_DEPENDS =		devel/py-six${MODPY_FLAVOR} \
			www/py-requests${MODPY_FLAVOR} \
			devel/py-decorator${MODPY_FLAVOR} \
			www/py-beautifulsoup4${MODPY_FLAVOR} \
			devel/py-kitchen${MODPY_FLAVOR}

NO_TEST =		Yes

.include <bsd.port.mk>
