# $OpenBSD: Makefile.template,v 1.76 2017/02/25 16:04:20 danj Exp $

COMMENT =	helpful python snippets packed into a library

MODPY_EGG_VERSION =	1.2.5
DISTNAME =	kitchen-${MODPY_EGG_VERSION}
PKGNAME =	py-kitchen-${MODPY_EGG_VERSION}

GH_ACCOUNT =	fedora-infra
GH_PROJECT =	kitchen
GH_TAGNAME =	v${MODPY_EGG_VERSION}

CATEGORIES =	devel

MAINTAINER =		Florian Stinglmayr <florian@n0la.org>

# LGPLv2+
PERMIT_PACKAGE_CDROM =	Yes

FLAVORS =		python3
FLAVOR ?=

MODULES =		lang/python

MODPY_SETUPTOOLS =	Yes

# Has no test suite
NO_TEST =		Yes

.include <bsd.port.mk>
