<!DOCTYPE html>
<html lang="en">
<head>
<!--     <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> -->
<!--     <title>BigNumber Library</title>
    <style>
        body { font-family: Arial, sans-serif; line-height: 1.6; margin: 0; padding: 0; background-color: #f9f9f9; color: #333; }
        header { background-color: #0078d7; color: white; padding: 1rem 0; text-align: center; }
        main { max-width: 800px; margin: 2rem auto; padding: 1rem; background: white; box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); }
        h1, h2, h3 { color: #0078d7; }
        code { background: #f4f4f4; padding: 0.2rem 0.4rem; border-radius: 5px; }
        pre { background: #f4f4f4; padding: 1rem; border-left: 5px solid #0078d7; overflow-x: auto; }
        footer { text-align: center; margin-top: 2rem; font-size: 0.8rem; color: #777; }
    </style> -->
</head>
<body>
    <header>
        <h1>Big Real Application</h1>
        <p>Handle large decimal and real numbers with ease.</p>
    </header>
    <main>
        <section>
            <h2>Features</h2>
            <h3>BigDecimalInt Class</h3>
            <ul>
                <li><strong>Purpose:</strong> Handles large integer operations.</li>
                <li><strong>Key Operations:</strong>
                    <ul>
                        <li>Addition (<code>+</code>)</li>
                        <li>Subtraction (<code>-</code>)</li>
                        <li>Comparisons (<code>&lt;</code>, <code>&gt;</code>, <code>==</code>)</li>
                        <li>Assignment (<code>=</code>)</li>
                        <li>Size and sign determination</li>
                    </ul>
                </li>
                <li><strong>Input Validation:</strong> Ensures valid numerical input.</li>
                <li><strong>Integration:</strong> Outputs data with overloaded stream operators (<code>&lt;&lt;</code>).</li>
            </ul>
            <h3>BigReal Class</h3>
            <ul>
                <li><strong>Purpose:</strong> Extends functionality to large floating-point numbers.</li>
                <li><strong>Key Features:</strong>
                    <ul>
                        <li>Handles integer and fractional parts separately.</li>
                        <li>Arithmetic operations: Addition (<code>+</code>), Subtraction (<code>-</code>).</li>
                        <li>Comparisons (<code>&lt;</code>, <code>&gt;</code>, <code>==</code>).</li>
                        <li>Assignment and move semantics.</li>
                    </ul>
                </li>
                <li><strong>Constructors:</strong> Supports string, double, and <code>BigDecimalInt</code>.</li>
                <li><strong>Stream Operations:</strong> Input (<code>&gt;&gt;</code>) and Output (<code>&lt;&lt;</code>).</li>
            </ul>
        </section>
        <section>
            <h2>Usage</h2>
            <h3>Include the Library</h3>
            <pre>#include "BigNumber.h"</pre>
            <h3>Example Code</h3>
            <pre>
#include "BigNumber.h"
#include &lt;iostream&gt;

int main() {
    BigDecimalInt num1("12345678901234567890");
    BigDecimalInt num2("98765432109876543210");

    BigDecimalInt sum = num1 + num2;
    std::cout &lt;&lt; "Sum: " &lt;&lt; sum &lt;&lt; std::endl;

    BigReal real1("1234.5678");
    BigReal real2("8765.4321");

    BigReal difference = real1 - real2;
    std::cout &lt;&lt; "Difference: " &lt;&lt; difference &lt;&lt; std::endl;

    return 0;
}
            </pre>
            <h3>Compilation</h3>
            <pre>g++ -o BigNumberTest main.cpp BigNumber.h</pre>
        </section>
        <section>
            <h2>Supported Platforms</h2>
            <ul>
                <li>Windows</li>
                <li>macOS</li>
                <li>Linux</li>
            </ul>
        </section>
        <section>
            <h2>Future Work</h2>
            <ul>
                <li>Optimization for large-scale computations.</li>
                <li>Additional operations such as multiplication and division.</li>
                <li>Enhanced error handling and input parsing.</li>
            </ul>
        </section>
        <section>
            <h2>Contributions</h2>
            <p>Contributions are welcome! Feel free to fork the repository and submit pull requests.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2025 BigNumber Library. All rights reserved.</p>
    </footer>
</body>
</html>
