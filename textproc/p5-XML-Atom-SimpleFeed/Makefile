# $NetBSD: Makefile,v 1.31 2021/05/24 19:54:49 wiz Exp $

DISTNAME=	XML-Atom-SimpleFeed-0.904
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	2
CATEGORIES=	textproc perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=XML/}

MAINTAINER=	kleink@NetBSD.org
HOMEPAGE=	https://metacpan.org/release/XML-Atom-SimpleFeed
COMMENT=	Generate simple Atom syndication feeds
LICENSE=	${PERL5_LICENSE}

PERL5_PACKLIST=		auto/XML/Atom/SimpleFeed/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
