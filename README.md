# Week-6-Programming
Week 6 Programming Code

//Ryan Bain
//ITD-1253-60498 Object Oriented Using C#
//10-18-2022
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Module6MethodsProjectDL
{
    public partial class Form1 : Form
    {
        // Public Contsants to use
        const byte ADD = 0;
        const byte SUBTRACT = 1;
        const byte MULTIPLY = 2;
        const byte DIVIDE = 3;
        const byte MODULUS = 4;

        public Form1()
        {
            InitializeComponent();
        }

        //Put Your method here

        private void btn5_Click(object sender, EventArgs e)
        {
            decimal dLeft = 0.0m;
            decimal dRight = 0.0m;
            decimal dAnswer = 0.0m;
            string szLeft = "";
            string szRight = "";
            string szAnswer = "";
            string szEquation = "";

            szLeft = textBox2.Text;
            szRight = textBox1.Text;

            dLeft = Convert.ToDecimal(szLeft);
            dRight = Convert.ToDecimal(szRight);

            dAnswer = dLeft % dRight;

            szAnswer = dAnswer.ToString();

            szEquation = szLeft + " % " + szRight + " = " + szAnswer;

            label3.Text = "";
            label3.Text = szEquation;


        }

        public static float AM_Operations(int FirstNumber, int SecondNumber, string Operator)
        {
            float result = 0;
            if (Operator == "+")
            {
                result = SecondNumber + FirstNumber;
            }
            else if (Operator == "-")
            {
                result = SecondNumber - FirstNumber;
            }
            else if (Operator == "*")
            {
                result = SecondNumber * FirstNumber;
            }
            else if (Operator == "/")
            {
                result = FirstNumber / SecondNumber;
            }
            else
            {
                result = FirstNumber % SecondNumber;
            }
            return result;
        }


        private void btn4_Click(object sender, EventArgs e)
        {
            decimal dLeft = 0.0m;
            decimal dRight = 0.0m;
            decimal dAnswer = 0.0m;
            string szLeft = "";
            string szRight = "";
            string szAnswer = "";
            string szEquation = "";

            szLeft = textBox2.Text;
            szRight = textBox1.Text;

            dLeft = Convert.ToDecimal(szLeft);
            dRight = Convert.ToDecimal(szRight);

            dAnswer = dLeft / dRight;

            szAnswer = dAnswer.ToString();

            szEquation = szLeft + " / " + szRight + " = " + szAnswer;

            label3.Text = "";
            label3.Text = szEquation;


        }

        private void btn3_Click(object sender, EventArgs e)
        {
            decimal dLeft = 0.0m;
            decimal dRight = 0.0m;
            decimal dAnswer = 0.0m;
            string szLeft = "";
            string szRight = "";
            string szAnswer = "";
            string szEquation = "";

            szLeft = textBox2.Text;
            szRight = textBox1.Text;

            dLeft = Convert.ToDecimal(szLeft);
            dRight = Convert.ToDecimal(szRight);

            dAnswer = dLeft * dRight;

            szAnswer = dAnswer.ToString();

            szEquation = szLeft + " * " + szRight + " = " + szAnswer;

            label3.Text = "";
            label3.Text = szEquation;


        }

        private void btn2_Click(object sender, EventArgs e)
        {
            decimal dLeft = 0.0m;
            decimal dRight = 0.0m;
            decimal dAnswer = 0.0m;
            string szLeft = "";
            string szRight = "";
            string szAnswer = "";
            string szEquation = "";

            szLeft = textBox2.Text;
            szRight = textBox1.Text;

            dLeft = Convert.ToDecimal(szLeft);
            dRight = Convert.ToDecimal(szRight);

            dAnswer = dLeft - dRight;

            szAnswer = dAnswer.ToString();

            szEquation = szLeft + " - " + szRight + " = " + szAnswer;

            label3.Text = "";
            label3.Text = szEquation;


        }

        private void btn1_Click(object sender, EventArgs e)
        {
            decimal dLeft = 0.0m;
            decimal dRight = 0.0m;
            decimal dAnswer = 0.0m;
            string szLeft = "";
            string szRight = "";
            string szAnswer = "";
            string szEquation = "";

            szLeft = textBox2.Text;
            szRight = textBox1.Text;

            dLeft = Convert.ToDecimal(szLeft);
            dRight = Convert.ToDecimal(szRight);

            dAnswer = dLeft + dRight;

            szAnswer = dAnswer.ToString();

            szEquation = szLeft + " + " + szRight + " = " + szAnswer;

            label3.Text = "";
            label3.Text = szEquation;

        }

        private void txtBox2_TextChanged(object sender, EventArgs e)
        {

        }

        private void lbl1_Click(object sender, EventArgs e)
        {

        }

        private void txtBox1_TextChanged(object sender, EventArgs e)
        {

        }

        private void lbl3_Click(object sender, EventArgs e)
        {

        }

        private void lbl2_Click(object sender, EventArgs e)
        {

        }

        private void btn6_Click(object sender, EventArgs e)
        {
            this.Close();
        }
    }
}
