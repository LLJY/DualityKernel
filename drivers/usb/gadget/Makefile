#
# USB peripheral controller drivers
#
subdir-ccflags-$(CONFIG_USB_GADGET_DEBUG)	:= -DDEBUG
subdir-ccflags-$(CONFIG_USB_GADGET_VERBOSE)	+= -DVERBOSE_DEBUG
ccflags-y				+= -I$(srctree)/drivers/usb/gadget/udc -I$(srctree)/drivers/usb/gadget/function

obj-$(CONFIG_USB_LIBCOMPOSITE)	+= libcomposite.o
libcomposite-y			:= usbstring.o config.o epautoconf.o
libcomposite-y			+= composite.o functions.o u_f.o

obj-y				+= debug.o
<<<<<<< HEAD
g_android-y			:= android.o function/f_hid.o
CFLAGS_android.o := -I$(src)
=======
g_android-y			:= android.o
>>>>>>> 132f55c417fd9d9f65c56927b69313b211be9353

obj-$(CONFIG_USB_GADGET)	+= udc/ function/ legacy/

obj-$(CONFIG_USB_G_ANDROID)	+= g_android.o

obj-$(CONFIG_USB_CI13XXX_MSM)	+= ci13xxx_msm.o

obj-$(CONFIG_USB_CI13XXX_MSM_HSIC)	+= ci13xxx_msm_hsic.o
