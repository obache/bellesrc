# $NetBSD: Makefile,v 1.12 2021/05/03 19:01:20 pho Exp $

DISTNAME=	xmonad-contrib-0.16
PKGNAME=	${DISTNAME}
PKGREVISION=	2
CATEGORIES=	wm

MAINTAINER=	degroote@NetBSD.org
COMMENT=	Third party extensions for xmonad
LICENSE=	modified-bsd

.include "options.mk"

.include "../../devel/hs-extensible-exceptions/buildlink3.mk"
.include "../../devel/hs-old-locale/buildlink3.mk"
.include "../../time/hs-old-time/buildlink3.mk"
.include "../../devel/hs-random/buildlink3.mk"
.include "../../math/hs-semigroups/buildlink3.mk"
.include "../../devel/hs-utf8-string/buildlink3.mk"
.include "../../x11/hs-X11/buildlink3.mk"
.include "../../wm/xmonad/buildlink3.mk"
.include "../../mk/haskell.mk"
.include "../../mk/bsd.pkg.mk"
