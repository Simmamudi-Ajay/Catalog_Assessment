# Shamir's Secret Sharing Implementation

This project solves a simplified version of **Shamir's Secret Sharing** using **Lagrange Interpolation** to find the constant term `c` of a polynomial. It decodes the polynomial's encoded roots (given in various number bases) and determines the secret constant using a set of at least `k` decoded points. The project reads a JSON file for input and outputs the secret constant term.

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Simmamudi-Ajay/Catalog_Assessment.git

## Test Cases

### Test Case 1

**Input:**
```json
{
    "keys": {
        "n": 4,
        "k": 3
    },
    "1": {
        "base": "10",
        "value": "4"
    },
    "2": {
        "base": "2",
        "value": "111"
    },
    "3": {
        "base": "10",
        "value": "12"
    },
    "6": {
        "base": "4",
        "value": "213"
    }
}
```

**Output:**
```
Secret for Test Case 1: 3
```

---

### Test Case 2

**Input:**
```json
{
    "keys": {
        "n": 10,
        "k": 7
    },
    "1": {
        "base": "6",
        "value": "13444211440455345511"
    },
    "2": {
        "base": "15",
        "value": "aed7015a346d63"
    },
    "3": {
        "base": "15",
        "value": "6aeeb69631c227c"
    },
    "4": {
        "base": "16",
        "value": "e1b5e05623d881f"
    },
    "5": {
        "base": "8",
        "value": "316034514573652620673"
    },
    "6": {
        "base": "3",
        "value": "2122212201122002221120200210011020220200"
    },
    "7": {
        "base": "3",
        "value": "20120221122211000100210021102001201112121"
    },
    "8": {
        "base": "6",
        "value": "20220554335330240002224253"
    },
    "9": {
        "base": "12",
        "value": "45153788322a1255483"
    },
    "10": {
        "base": "7",
        "value": "1101613130313526312514143"
    }
}
```

**Output:**
```
Secret for Test Case 2: 79836264046592
```
```

