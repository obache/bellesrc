# $NetBSD: Makefile,v 1.19 2020/01/26 17:31:49 rillig Exp $
#

DISTNAME=	ftpproxy-${VERSION}
CATEGORIES=	net
MASTER_SITES=	http://www.ftpproxy.org/download/
MASTER_SITES+=	http://www.ftpproxy.org/download/older_releases/
EXTRACT_SUFX=	.tgz

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://www.ftpproxy.org/
COMMENT=	Application level gateway for FTP

BUILD_DIRS=	src
VERSION=	1.2.3

.include "../../mk/bsd.prefs.mk"

MAKE_ENV+=	OSLIB=${LIBS:M*:Q} VERSION=${VERSION:Q}

LIBS.SunOS+=		-lsocket -lnsl
MAKE_ENV.SunOS+=	OSFLAG=-DSOLARIS

INSTALLATION_DIRS=	libexec ${PKGMANDIR}/man8

do-install:
	${INSTALL_PROGRAM} ${WRKSRC:Q}/src/ftp.proxy ${DESTDIR}${PREFIX}/libexec/
	${INSTALL_MAN} ${WRKSRC:Q}/doc/ftp.proxy.1 ${DESTDIR}${PREFIX}/${PKGMANDIR}/man8/ftp.proxy.8

.include "../../mk/bsd.pkg.mk"
