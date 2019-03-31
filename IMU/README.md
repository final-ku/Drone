#### 19/03/29 imu list

------

**IMU 센서 조사**

: dji의 flight controller, px4의 flight controller, 갤럭시, 아이폰에서 사용되는 imu 센서



------

| model     | imu sensor        | interface | github code                                                  |
| :-------- | ----------------- | --------- | ------------------------------------------------------------ |
| DJI A3    |                   |           | x                                                            |
| Pix4      | MPU6000           | spi,i2c   | x                                                            |
| Galaxy S6 | MPU6500           | spi,i2c   | x                                                            |
| Galaxy S7 | LSM6DS3           | spi,i2c   | <https://github.com/search?l=Python&q=LSM6DS3&type=Repositories> |
| Galaxy S8 | LSM6DL            |           | x                                                            |
| Galaxy S9 | LSM6DSL           | spi,i2c   | x                                                            |
| iphone 6  | MPU-6500 / BMA280 | spi,i2c   | x                                                            |
| iphone 7  | LSM6DSM           |           | x                                                            |
| iphone X  | BMI160 변형       |           | x                                                            |

MPU6050 :   <https://github.com/search?l=Python&q=MPU6050&type=Repositories>



- 빈 공간으로 되어있는 센서들은 애초에 센서 정보를 비공개 해놓았거나 github에 소스 정보가 없는 것들.
- github에 python 코드를 포함하고 있는 imu 센서는 **Galaxy S7의 LSM6DS3** 하나 뿐이였고,  나머지는 소스코드가 아에 없거나 c나 c++로 구성되있음.
- LSM 시리즈와 같이 자주 사용되고있는 MPU6500의 경우에는 github에 python 소스코드가 존재하지 않지만 하위버전인 MPU6050의 코드는 정보량이 LSM6DS3의 배수로 많음.  
