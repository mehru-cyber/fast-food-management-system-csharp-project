# fast-food-management-system-csharp-project
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace fastfoodresturant
{
    public partial class closelbl : Form
    {
        public closelbl()
        {
            InitializeComponent();
        }

        private void flowLayoutPanel1_Paint(object sender, PaintEventArgs e)
        {

        }

        private void panel3_Paint(object sender, PaintEventArgs e)
        {

        }

        private void panel4_Paint(object sender, PaintEventArgs e)
        {

        }

        private void label2_Click(object sender, EventArgs e)
        {

        }

        private void pictureBox1_Click(object sender, EventArgs e)
        {

        }

        private void panel2_Paint(object sender, PaintEventArgs e)
        {
            if (PizzaCb.Checked == true)
            { PizzaTb.Enabled = true; }
            if(PizzaCb.Checked == false)
            { PizzaTb.Enabled = false;
                PizzaTb.Text = "0";
            }
            
        }

        private void label4_Click(object sender, EventArgs e)
        {

        }

        private void Form1_Load(object sender, EventArgs e)
        {
            
        }

        private void checkBox6_CheckedChanged(object sender, EventArgs e)
        {
            if (DrumstiCb.Checked == true)
            { DrumstiTb.Enabled = true; }
            if (DrumstiCb.Checked == false)
            {
                DrumstiTb.Enabled = false;
                DrumstiTb.Text = "0";
            }
        }

        private void label9_Click(object sender, EventArgs e)
        {

        }

        private void ColaCb_CheckedChanged(object sender, EventArgs e)
        {

        }

        private void PizzaCb_CheckedChanged(object sender, EventArgs e)
        {

        }

        private void TeaCb_CheckedChanged(object sender, EventArgs e)
        {

        }

        private void panel5_Paint(object sender, PaintEventArgs e)
        {

        }

        private void WrapCb_CheckedChanged(object sender, EventArgs e)
        {
            if (WrapCb.Checked == true)
            { WrapTb.Enabled = true; }
            if (WrapCb.Checked == false)
            {
                WrapTb.Enabled = false;
                WrapTb.Text = "0";
            }
        }

        private void SlaadCb_CheckedChanged(object sender, EventArgs e)
        {
            if (SlaadCb.Checked == true)
            { SaladTb.Enabled = true; }
            if (SlaadCb.Checked == false)
            {
                SaladTb.Enabled = false;
                SaladTb.Text = "0";
            }
        }

        private void SandwichCb_CheckedChanged(object sender, EventArgs e)
        {

        }

        private void WaterCb_CheckedChanged(object sender, EventArgs e)
        {

        }

        private void panel3_Paint_1(object sender, PaintEventArgs e)
        {

        }

        private void PastaCb_CheckedChanged(object sender, EventArgs e)
        {
            if (PastaCb.Checked == true)
            { PastaTb.Enabled = true; }
            if (PastaCb.Checked == false)
            {
                PastaTb.Enabled = false;
                PastaTb.Text = "0";
            }
        }

        private void label18_Click(object sender, EventArgs e)
        {
            Application.Exit();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            PizzaCb.Checked = false;
            WrapCb.Checked = false;
            SlaadCb.Checked = false;
            SandwichCb.Checked = false;
            DrumstiCb.Checked = false;
            PastaCb.Checked = false;
            TeaCb.Checked = false;
            ColaCb.Checked = false;
            WaterCb.Checked = false;
            ChoclateCb.Checked = false;
            CakeCb.Checked = false;
        }
        
        double pizzaup = 5000, pastaup = 80, slaadup = 50, sandwichup = 100, drumsti = 150, pasta = 500;
        double teaup = 70, colaup = 200, waterup = 70, chocolateup = 150, pancakeup = 700, cakeup = 3000;

        private void label23_Click(object sender, EventArgs e)
        {

        }

        private void label24_Click(object sender, EventArgs e)
        {

        }

        private void printPreviewDialog1_Load(object sender, EventArgs e)
        {
        }

        private void label19_Click(object sender, EventArgs e)
        {

        }

        private void label22_Click(object sender, EventArgs e)
        {

        }

        private void button3_Click(object sender, EventArgs e)
        {
            if (printPreviewDialog1.ShowDialog() == DialogResult.OK)
            {
                printDocument1.Print();
            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            if(PizzaCb.Checked == true) {
                ReceiptTb.AppendText("\tPizza;\t" + pizzatp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + pizzatp;
                Subtotallbl.Text = "" + Subtotal;
            }
            if (WrapCb.Checked == true)
            {
                ReceiptTb.AppendText("\tWrap;\t" + wraptp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + wraptp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (SlaadCb.Checked == true)
            {
                ReceiptTb.AppendText("\tSalad;\t" + saladtp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + saladtp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (SandwichCb.Checked == true)
            {
                ReceiptTb.AppendText("\tSandwich;\t" + sandwichtp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + sandwichtp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (DrumstiCb.Checked == true)
            {
                ReceiptTb.AppendText("\tDrumsti;\t" + drumstitp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + drumstitp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (PastaCb.Checked == true)
            {
                ReceiptTb.AppendText("\tPasta;\t" + pastatp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + pastatp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (TeaCb.Checked == true)
            {
                ReceiptTb.AppendText("\tTea;\t" + teatp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + teatp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (ColaCb.Checked == true)
            {
                ReceiptTb.AppendText("\tCola;\t" + colatp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + colatp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (WaterCb.Checked == true)
            {
                ReceiptTb.AppendText("\tWater;\t" + watertp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + watertp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (ChoclateCb.Checked == true)
            {
                ReceiptTb.AppendText("\tChocolate;\t" + chocolatetp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + chocolatetp;
                Subtotallbl.Text = "" + Subtotal;

            }
            if (CakeCb.Checked == true)
            {
                ReceiptTb.AppendText("\tCake;\t" + caketp + "Rs" + Environment.NewLine);
                    Subtotal = Subtotal + caketp;
                Subtotallbl.Text = "" + Subtotal;

            }
            

        }

        double pizzatp, wraptp, saladtp, sandwichtp, drumstitp, pastatp, teatp, colatp, watertp, chocolatetp, pancaketp, caketp;
        double Subtotal = 0;
        private object wrapTp;
        private double saladup;

        public object PizzaTp { get; private set; }
        public object SandwichTb { get; private set; }
        public float ReferenceSansSerif { get; private set; }

        private void panel6_Paint(object sender, PaintEventArgs e)
        {
            pizzatp = pizzaup * Convert.ToDouble(PizzaTb.Text);
            wraptp = pastaup * Convert.ToDouble(WrapTb.Text);
            saladtp = saladup * Convert.ToDouble(SaladTb.Text);
 
            drumstitp = pastaup * Convert.ToDouble(DrumstiTb.Text);
            pastatp = pastaup * Convert.ToDouble(PastaTb.Text);
            
            ReceiptTb.Clear();
            Subtotal = 0;
            ReceiptTb.AppendText(Environment.NewLine);
            ReceiptTb.AppendText("\t\t\tCODESPACE RESTURENT\t\t"+Environment.NewLine);
            ReceiptTb.AppendText("\t\t\t*"+Environment.NewLine);




        }

        private void ReceiptTb_TextChanged(object sender, EventArgs e)
        

  
    }
}
