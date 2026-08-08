ESP-NOW with ESP-C3-32S-Kit: Quick Briefing
What We Built:
Wireless Light Controller using ESP-NOW protocol:
• ESP #1: LDR sensor → Sends "ON" when dark, "OFF" when light
• ESP #2: Receives commands → Controls LED
• Communication: Broadcast to 0xFF:FF:FF:FF:FF:FF (all devices)
Key Components:
Hardware:
• 2× ESP-C3-32S-Kit boards
• LDR + 10K resistor (voltage divider) → GPIO4
• LED + 220Ω resistor → GPIO5
• Breadboard + jumper wires
Software:
• Protocol: ESP-NOW (Espressif's proprietary 2.4GHz)
• Library: #include esp_now.h
• Platform: Arduino Framework on ESP32-C3
