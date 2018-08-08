use employees_mod;
SELECT 
    YEAR(tde.from_date) AS joining_year,
    te.gender,
    COUNT(te.emp_no) AS emp_count
FROM
    t_employees te
        JOIN
    t_dept_emp tde ON te.emp_no = tde.emp_no
GROUP BY joining_year , te.gender
HAVING joining_year >= 1990
ORDER BY joining_year, te.gender;
