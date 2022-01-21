if (TARGET tinyusb_device)
        set(FAMILY rp2040)
        set(BOARD pico_sdk)
        set(TINYUSB_FAMILY_PROJECT_NAME_PREFIX "tinyusb_dev_")

        add_subdirectory(pico)
else ()
        message(WARNING "TinyUSB required, not found!")
        message(WARNING "Not building Pico side!")
endif ()

# Kernel module stuff here ???
