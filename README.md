# TUK-SKT Industrial Datasets for Machine Learning
---
- TSID ( [TUK] - [SKT] Industrial Datasets ) is dataset for studying, benchmarking, etc., mainly in machine learning and smart-factory field. It contains multiple type of real simulation asset’s data. All dataset is collected from well-designed experiments.
- Currently, two types of asset is opend. More types will be opend soon.

## Datasets
---
| Asset Type | URL |Data Contents | Format |
| ------ | ------ | ------ | ------ |
| Stamping Press Machine | ... | Stamped Coin Quality Data : 40 rows  | csv |
| Conveyor Belt System | ... | Normal Belt : 900 rows <br/> Cut-diagonal Belt : 900 rows <br/> Cut-vertical Belt : 900 rows <br/> Cut-vetrical-multiple Belt : 900 rows <br/> Cut-vertical-diagonal Belt : 900 rows | csv |

#### Stamping Press Machine
- The machine presses the aluminum coin to print a specific pattern.
- 5 types of data ( Pressure Limit, Actual Pressure, Adjust Speed, Deceleration Distatnce, Quality Score ) were collected every trials.
- _Data Field Description_
    - Pressure Limit
        - Configured value. The machine presses the coin with a specific pressure as per the pressure limit value.
    - Actual Pressure
        - Measured value. It was measured by the pressure sensor at pressing the coin.
    - Adjust Speed
        - Configured value.The machine presses the coin with a specific speed as per the adjust speed value.
    - Deceleration Distance
        - Configured value. The machine decelerates press speed when the distance between punch surface and coin surface are closer to a specific value as per the deceleration distance value.
    - Quality Score
        - Measured value. We measured the quality score applying canny edge method on a stamped coin picture.
        
#### Conveyor Belt System


## License
MIT

   [TUK]: <https://www.tukorea.ac.kr/tukorea/index.do>
   [SKT]: <http://b2b.tworld.co.kr/bizts/solution/solutionTemplate.bs?solutionId=0088>
