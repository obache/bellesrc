# $NetBSD: Makefile,v 1.21 2021/05/24 19:50:58 wiz Exp $

DISTNAME=	Log-Dispatch-DBI-0.02
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	15
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Log/}

MAINTAINER=	pkgsrc-users@NetBSD.org
COMMENT=	Perl module for logging messages via the DBI interface

DEPENDS+=	p5-DBD-CSV-[0-9]*:../../databases/p5-DBD-CSV
DEPENDS+=	p5-Log-Dispatch-[0-9]*:../../devel/p5-Log-Dispatch

USE_LANGUAGES=	# empty

PERL5_PACKLIST=	auto/Log/Dispatch/DBI/.packlist

.include "../../databases/p5-DBI/buildlink3.mk"

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
