# $FreeBSD$

PORTNAME=	libgrading
PORTVERSION=	0.1.2
DISTVERSIONPREFIX=	v
CATEGORIES=	devel

MAINTAINER=	jonathan@FreeBSD.org
COMMENT=	Simple library for grading C- and C++-language assignments

LICENSE=	APACHE20

LIB_DEPENDS=	libdistance.so:devel/libdistance

USE_GITHUB=	yes
GH_ACCOUNT=	trombonehero

USES=		cmake
USE_LDCONFIG=	yes

PLIST_FILES=	include/libgrading.h \
		lib/libgrading.so

.include <bsd.port.mk>
