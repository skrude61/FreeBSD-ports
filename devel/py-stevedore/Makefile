# Created by: Nicola Vitale <nivit@FreeBSD.org>
# $FreeBSD$

PORTNAME=	stevedore
PORTVERSION=	1.17.1
CATEGORIES=	devel
MASTER_SITES=	CHEESESHOP
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	nivit@FreeBSD.org
COMMENT=	Manage dynamic plugins for Python applications

LICENSE=	APACHE20

BUILD_DEPENDS=	${PKGNAMEPREFIX}pbr>=1.6:devel/py-pbr # <2.0
RUN_DEPENDS=	${PKGNAMEPREFIX}argparse>=1.2.1:devel/py-argparse \
		${PKGNAMEPREFIX}pbr>=1.6:devel/py-pbr \
		${PKGNAMEPREFIX}six>=1.9.0:devel/py-six

USES=		python
USE_PYTHON=	autoplist distutils

.include <bsd.port.mk>
