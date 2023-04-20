# SW Build for Adafruit Feather 32u4 LoRa Radio (AVR Architecture)

Disable unused drivers in `RadioLib/src/BuildOpt.h`:
```
  //#define RADIOLIB_EXCLUDE_CC1101
  #define RADIOLIB_EXCLUDE_NRF24
  #define RADIOLIB_EXCLUDE_RF69
  #define RADIOLIB_EXCLUDE_SX1231     // dependent on RADIOLIB_EXCLUDE_RF69
  #define RADIOLIB_EXCLUDE_SI443X
  #define RADIOLIB_EXCLUDE_RFM2X      // dependent on RADIOLIB_EXCLUDE_SI443X
  //#define RADIOLIB_EXCLUDE_SX127X
  //#define RADIOLIB_EXCLUDE_RFM9X      // dependent on RADIOLIB_EXCLUDE_SX127X
  #define RADIOLIB_EXCLUDE_SX126X
  #define RADIOLIB_EXCLUDE_STM32WLX   // dependent on RADIOLIB_EXCLUDE_SX126X
  #define RADIOLIB_EXCLUDE_SX128X
  #define RADIOLIB_EXCLUDE_AFSK
  #define RADIOLIB_EXCLUDE_AX25
  #define RADIOLIB_EXCLUDE_HELLSCHREIBER
  #define RADIOLIB_EXCLUDE_MORSE
  #define RADIOLIB_EXCLUDE_RTTY
  #define RADIOLIB_EXCLUDE_SSTV
  #define RADIOLIB_EXCLUDE_DIRECT_RECEIVE
```