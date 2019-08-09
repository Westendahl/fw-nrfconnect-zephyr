# Copyright (c) 2019 Nordic Semiconductor ASA.
# Modifications Copyright (c) 2019 Actinius
# SPDX-License-Identifier: Apache-2.0

zephyr_library()
zephyr_library_sources(board.c)

if(CONFIG_BOARD_NRF52840_GPIO_RESET)
  zephyr_library_sources(nrf52840_reset.c)
endif()


