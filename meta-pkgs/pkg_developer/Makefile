# $NetBSD: Makefile,v 1.9 2020/08/30 08:22:39 tnn Exp $
#

DISTNAME=	pkg_developer-1.2.2
CATEGORIES=	meta-pkgs pkgtools
MASTER_SITES=	# empty
DISTFILES=	# empty

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://www.pkgsrc.org/
COMMENT=	Meta-package for pkgsrc package development

META_PACKAGE=	yes

DEPENDS+=	checkperms>=1.0:../../sysutils/checkperms
DEPENDS+=	createbuildlink>=3.13:../../pkgtools/createbuildlink
DEPENDS+=	digest>=20060302:../../pkgtools/digest
DEPENDS+=	import-package>=1.0:../../pkgtools/import-package
DEPENDS+=	lintpkgsrc>=4.82:../../pkgtools/lintpkgsrc
DEPENDS+=	pkg_chk>=1.77:../../pkgtools/pkg_chk
DEPENDS+=	pkg_tarup>=1.6.5:../../pkgtools/pkg_tarup
DEPENDS+=	pkgdiff>=0.119:../../pkgtools/pkgdiff
.include "../../pkgtools/pkglint/select.mk"
DEPENDS+=	revbump>=1.8:../../pkgtools/revbump
DEPENDS+=	url2pkg>=1.34:../../pkgtools/url2pkg
DEPENDS+=	verifypc>=1.3:../../pkgtools/verifypc

.include "../../mk/bsd.pkg.mk"
