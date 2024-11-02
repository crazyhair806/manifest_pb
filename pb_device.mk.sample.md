<a href="README.md" >Go Back</a>

### pb_device.mk sample

```bash
# Inherit from those products. Most specific first.
$(call inherit-product, $(SRC_TARGET_DIR)/product/core_64_bit.mk) -- only for 64bit phones

# Inherit from device
$(call inherit-product, device/<path>/device.mk) -- path to main device makefile

# Inherit common product files.
$(call inherit-product, vendor/pb/config/common.mk)

# Set those variables here to overwrite the inherited values.
BOARD_VENDOR := 
PRODUCT_BRAND :=motorola 
PRODUCT_DEVICE := avatrn
PRODUCT_NAME := pb_device
PRODUCT_MANUFACTURER := motorola
PRODUCT_MODEL := motorola edge 2024
TARGET_VENDOR := 
