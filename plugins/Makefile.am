AUTOMAKE_OPTIONS = foreign
AM_CPPFLAGS = -I$(top_srcdir)/src

SUBDIRS  =

## image loading/saving plugins
SUBDIRS += imageMAGICK imageTIFF imageJPEG imageSGI imageQT


## film loading plugins
SUBDIRS += filmAVFoundation filmAVI filmAVIPLAY filmDS filmDarwin filmGMERLIN filmMPEG1 filmMPEG3 filmQT filmQT4L
if DISABLED
SUBDIRS += filmTEST
SUBDIRS += videoTEST
endif

## Pix output (continuous) plugins
SUBDIRS += recordQT recordQT4L recordV4L recordV4L2

## video capture plugins
SUBDIRS += videoDC1394 videoDS videoDV4L videoDarwin videoSGI videoUNICAP
SUBDIRS += videoV4L videoV4L2 videoVFW videoVLC

## proprietary video capture plugins
SUBDIRS += videoAVT videoHALCON videoPYLON

## asset loading plugins
SUBDIRS += modelOBJ modelASSIMP2


## filmTEST is not built by default, but we want to ship it
DIST_SUBDIRS = $(SUBDIRS) filmTEST videoTEST

