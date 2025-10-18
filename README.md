If it crashes, type `bt` (backtrace) to see the call stack.
3. **Check COBOL code for:**
   - Array out-of-bounds access
   - Invalid `MOVE` operations (e.g., moving alphanumeric to numeric field)
   - Uninitialized variables used in calculations

---

### Data & Logic Issues

#### ❌ Incorrect salary calculations

**Problem:** Output values for gross/net salary, tax, or overtime are wrong.

**Solutions:**
1. **Review `payroll.cbl`:** Examine the calculation logic carefully.
2. **Check input data:** Ensure `employee.dat` and manual inputs (e.g., overtime hours) are correct.
3. **Debug step-by-step:** Use `DISPLAY` statements at intermediate calculation steps to trace values.

#### ❌ Data not saving or loading correctly

**Problem:** Employee records or payroll transactions are not persistent.

**Solutions:**
1. **Check file I/O operations:** Review `employee.cbl` and `payroll.cbl` for `OPEN`, `READ`, `WRITE`, `REWRITE`, `CLOSE` statements.
2. **Verify file status:** After each I/O operation, check the `FILE STATUS` variable. A value of `00` means success.
3. **Examine data files:** Open `employee.dat` and `payroll.dat` with a text editor to see if data is being written in the expected format.

---

## 📃 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙋‍♂️ Support

For any issues or questions, please open an issue on the GitHub repository. Your contributions and feedback are welcome!