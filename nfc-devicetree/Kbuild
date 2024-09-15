ifneq (,$(filter AI2205,$(ASUS_BUILD_PROJECT)))
$(warning [Build] dtbo for AI2205 8550 nfc...)

dtbo-y += nxp/kalama-nfc.dtbo \
	  nxp/AI2205-8550-EVB-nfc-overlay.dtbo \
	  nxp/AI2205-8550-SR1-nfc-overlay.dtbo \
	  nxp/AI2205-8550-SR2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-ER1-nfc-overlay.dtbo \
	  nxp/AI2205-8550-ER2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-PR-nfc-overlay.dtbo \
	  nxp/AI2205-8550-MP-nfc-overlay.dtbo

dtbo-y += nxp/kalama-v2-nfc.dtbo \
	  nxp/AI2205-8550-EVB-v2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-SR1-v2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-SR2-v2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-ER1-v2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-ER2-v2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-PR-v2-nfc-overlay.dtbo \
	  nxp/AI2205-8550-MP-v2-nfc-overlay.dtbo

else

dtbo-y += nxp/kalama-nfc.dtbo \
	  nxp/kalama-nfc-mtp.dtbo \
	  nxp/kalama-nfc-qrd.dtbo \
	  nxp/kalama-nfc-cdp.dtbo

dtbo-y += nxp/kalama-v2-nfc.dtbo \
	  nxp/kalama-v2-nfc-mtp.dtbo \
	  nxp/kalama-v2-nfc-qrd.dtbo \
	  nxp/kalama-v2-nfc-cdp.dtbo

dtbo-y += st/kalama-nfc.dtbo \
	  st/kalama-nfc-mtp.dtbo \
	  st/kalama-nfc-cdp.dtbo

dtbo-y += st/kalama-v2-nfc.dtbo \
	  st/kalama-v2-nfc-mtp.dtbo \
	  st/kalama-v2-nfc-cdp.dtbo
endif

ifeq ($(CONFIG_ARCH_KHAJE),y)
dtbo-y += nxp/khaje-nfc-idp.dtbo \
          nxp/khaje-nfc-qrd.dtbo \
          nxp/khaje-nfc-qrd-hvdcp3p5.dtbo \
          nxp/khaje-nfc-qrd-nowcd9375.dtbo
endif

always-y	:= $(dtb-y) $(dtbo-y)
subdir-y	:= $(dts-dirs)
clean-files	:= *.dtb *.dtbo
