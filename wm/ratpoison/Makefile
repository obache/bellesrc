# $NetBSD: Makefile,v 1.49 2021/05/24 19:55:10 wiz Exp $
#

DISTNAME=	ratpoison-1.4.9
PKGREVISION=	3
CATEGORIES=	wm
MASTER_SITES=	https://savannah.nongnu.org/download/ratpoison/
EXTRACT_SUFX=	.tar.xz

MAINTAINER=	tonio@NetBSD.org
HOMEPAGE=	https://www.nongnu.org/ratpoison/
COMMENT=	Simple window manager with no fat library dependencies
LICENSE=	gnu-gpl-v2

USE_TOOLS+=	perl:run pkg-config

GNU_CONFIGURE=	YES
INFO_FILES=	yes

REPLACE_PERL+=	contrib/rpws contrib/genrpbindings contrib/clickframe.pl
REPLACE_SH=	contrib/allwindows.sh

BUILDLINK_DEPMETHOD.libXt?=	build

.include "../../devel/readline/buildlink3.mk"
.include "../../x11/libX11/buildlink3.mk"
.include "../../x11/libXext/buildlink3.mk"
.include "../../x11/libXrandr/buildlink3.mk"
.include "../../x11/libXt/buildlink3.mk"
.include "../../x11/libXtst/buildlink3.mk"
.include "../../x11/libXft/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
