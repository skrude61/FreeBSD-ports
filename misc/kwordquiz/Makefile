# $FreeBSD$

PORTNAME=	kwordquiz
PORTVERSION=	${KDE4_VERSION}
CATEGORIES=	misc kde
MASTER_SITES=	KDE/${KDE4_BRANCH}/${PORTVERSION}/src
DIST_SUBDIR=	KDE/${PORTVERSION}

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Flash card trainer for KDE 4

USES=		cmake:outsource kde:4 tar:xz
USE_KDE=	kdelibs libkdeedu automoc4
USE_QT4=	moc_build qmake_build rcc_build uic_build

.include <bsd.port.mk>
