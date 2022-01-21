add_executable(fake_sd_pico)

target_sources(fake_sd_pico PUBLIC
        # Sources here
        )

target_include_directories(fake_sd_pico PUBLIC
        ${CMAKE_CURRENT_LIST_DIR}
        # More include dirs here
        )

target_link_libraries(fake_sd_pico PUBLIC
        pico_stdlib
        tinyusb_device
        tinyusb_board
        )

pico_add_extra_outputs(fake_sd_pico)
