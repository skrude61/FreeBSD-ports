# Created by: Conrad Meyer <cem@FreeBSD.org>
# $FreeBSD$

PORTNAME=	lkl
PORTVERSION=	4.5.0
CATEGORIES=	sysutils
PKGNAMEPREFIX=	fusefs-

MAINTAINER=	cem@FreeBSD.org
COMMENT=	Full-featured Linux BTRFS, Ext4, XFS as a FUSE module

LICENSE=	GPLv2

BUILD_DEPENDS=	gnubc>0:math/gnubc

USES=		fuse gmake python:build shebangfix
SHEBANG_FILES=	../../arch/lkl/scripts/headers_install.py
USE_BINUTILS=	yes
USE_GCC=	yes
USE_GITHUB=	yes
GH_PROJECT=	linux
GH_TAGNAME=	e145a5a5bdf4b70753495b5ccd2439a354655341

ONLY_FOR_ARCHS=	amd64
ONLY_FOR_ARCHS_REASON=No one has added other architecture ld formats yet

IGNORE_FreeBSD_9=	requires FreeBSD 11 or newer
IGNORE_FreeBSD_10=	requires FreeBSD 11 or newer

WRKSRC_SUBDIR=	tools/lkl
ALL_TARGET=	lklfuse
MAKE_JOBS_UNSAFE=yes
MAKE_ARGS+=	V=1
# Need ports versions of 'bc', 'ld' to build!
MAKE_ARGS+=	PATH="${LOCALBASE}/bin:${PATH}"

PLIST_FILES=	bin/lklfuse lib/liblkl.a

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/lklfuse ${STAGEDIR}${PREFIX}/bin
	${INSTALL_DATA} ${WRKSRC}/liblkl.a ${STAGEDIR}${PREFIX}/lib

.include <bsd.port.mk>
