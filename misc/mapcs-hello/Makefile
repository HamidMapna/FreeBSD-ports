# Created by: shipley@dis.org
# $FreeBSD$

PORTNAME=	mapcs-hello
PORTVERSION=	1.0
PORTREVISION=	1
CATEGORIES=	misc
MASTER_SITES=	#
DISTFILES=	#


MAINTAINER=	ports@mapcs.info
COMMENT=	Simple test port for pfSense package development

LICENSE=	BSD2CLAUSE

USES=		charsetfix perl5
USE_PERL5=	build

INFO=		hello

NO_CONFIGURE=    yes
NO_BUILD=	yes
NO_ARCH=	yes

OPTIONS_DEFINE=		NLS
OPTIONS_SUB=		yes

NLS_USES=		gettext
NLS_CONFIGURE_ENABLE=	nls
NLS_CPPFLAGS=		-I${LOCALBASE}/include
NLS_LDFLAGS=		-L${LOCALBASE}/lib

do-install:
	${INSTALL_SCRIPT} ${FILESDIR}/mapcs-hello.sh \
		${STAGEDIR}${PREFIX}/bin/mapcs-hello

.include <bsd.port.mk>
