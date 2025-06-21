# Age Input Field - Test Design  

**Field**: Age
**Valid Range**: 18-99

## Equivalence Partitioning

| Class Type  | Input Range  | Example Value | Valid/Invalid | 
|-------------|--------------|---------------|---------------|
| Below range | < 18         | 10            |  Invalid      |
| Valid Range | 18-99        | 50            |  Valid        |
| Above Range | > 99         | 110           |  Invalid      |
| Non-numeric | text/symbols | "aa"          |  Invalid      |
| Empty Input | (no value)   | -             |  Invalid      |

## Boundary Value Analysis

| Test Case             | Input    | Expected Result |
|-----------------------|----------|-----------------|
| Below lower boundary  | 17       | Invalid         |
| At lower boundary     | 18       | Valid           |
| Just above lower      | 19       | Valid           |
| Just below upper      | 98       | Valid           |
| At upper boundary     | 99       | Valid           |
| Above upper boundary  | 100      | Invalid         |
