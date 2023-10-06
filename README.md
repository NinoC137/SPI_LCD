# SPI_LCD
SPI LCD(ST7789) DMA(not completely DMA+frameBuffer)

实现了DMA+SPI刷屏的效果, 但是未能实现完全意义上的DMA+frameBuffer

目前仅利用DMA将刷屏次数降低至原先的1/8

疑问点:未能实现DMA一次性刷入大数组,进行了诸多测试,未能解决

## 配置注意事项:
1. SPI速率不能过快,否则可能无法成功初始化(ST7789最多支持到50MB/s)
2. GPIO要配置为超高速模式
3. 信号线加上拉电阻,尽量保证速率
