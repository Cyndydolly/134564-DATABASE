# 134564-DATABASE
CREATE TABLE Employee (
    emp_id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    birth_date DATE,
    sex CHAR(1),
    salary DECIMAL(10, 2),
    super_id INT,
    branch_id INT,
    FOREIGN KEY (super_id) REFERENCES Employee(emp_id)
);
