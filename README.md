# TUK-SKT Industrial Datasets for Machine Learning
- TSID ( [TUK] - [SKT] Industrial Datasets ) is a dataset for research, benchmarking, and more, mainly in machine learning and smart factory fields. It contains multiple type of real simulation asset’s data. All dataset is collected from well-designed experiments.
- Currently, two types of asset is opend. More types will be opend soon.

## Datasets
| Asset Type | URL | Contents | Format |
| ------ | ------ | ------ | ------ |
| Stamping Press Machine | https://github.com/yundhun/TSID/tree/main/stamping_press_machine | Stamped Coin Quality Data : 40 rows  | csv |
| Conveyor Belt System | ... | Normal Belt : 900 rows <br/> Cut-diagonal Belt : 900 rows <br/> Cut-vertical Belt : 900 rows <br/> Cut-vetrical-multiple Belt : 900 rows <br/> Cut-vertical-diagonal Belt : 900 rows | csv |

## Stamping Press Machine
<img width="640" alt="image" src="https://user-images.githubusercontent.com/15883027/189007516-cfc8ccde-7300-4c7d-813f-5aa567f91043.png">

- The machine presses the aluminum coin to print the specific pattern.
- 5 types of data ( Pressure Limit, Actual Pressure, Adjust Speed, Deceleration Distatnce, Quality Score ) were collected at every trials.
- Data Field Description
    | Field | Description |
    | ------ | ------ |
    | Pressure Limit | Configured value. The machine presses the coin with a specific pressure as per the pressure limit value. |
    | Actual Pressure | Measured value. It was measured by the pressure sensor at pressing the coin. |
    | Adjust Speed | Configured value.The machine presses the coin with a specific speed as per the adjust speed value. |
    | Deceleration Distance | Configured value. The machine decelerates press speed when the distance between punch surface and coin surface are closer to a specific value as per the deceleration distance value. |
    | Quality Score | Measured value. We measured the quality score applying canny edge method on a stamped coin picture. | 
        
## Conveyor Belt System
<img width="787" alt="image" src="https://user-images.githubusercontent.com/15883027/189014740-89f46ead-11dc-4739-b3a8-e8bab48f0dcd.png">

- The system consists of a motor, a belt, a bearing, and four types of sensors. Current, vibration, and noise sensors observe the condition of the motor. The distance sensor observes the deflection of the belt.
- 5 types of data ( Current, Vibration, Noise, Distatnce, Motor Speed ) were collected at every trials.
- Data Field Description
    | Field | Description |
    | ------ | ------ |
    | Current | Measured value. It was measured by the current sensor. (not shown at image) |
    | Vibration | Measured value. the vibration of the pulley part. It was measured by the vibration sensor. |
    | Noise | Measured value. the noise of the pulley part. It was measured by the noise sensor. |
    | Distatnce | Measured value. the distance between the sensor and the upper belt. It was measured by the laser distance sensor. |
    | Motor Speed | Measured value. the speed of the motor. It was measured by the speed sensor. (not shown at image) | 
    | Label | normal, diagonal, vertical. It means belt status. three types of labels are provided. *the bearing label will be added soon |

## License
MIT

   [TUK]: <https://www.tukorea.ac.kr/tukorea/index.do>
   [SKT]: <http://b2b.tworld.co.kr/bizts/solution/solutionTemplate.bs?solutionId=0088>
