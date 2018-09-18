using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp1
{
    class Pessoa
    {
        private string name;
        private float weight;
        private float high;
        private int age;
        private Data born;

        public Pessoa(string n, float w, float h, int a, Data bo)
        {
            name = n;
            weight = w;
            high = h;
            age = a;
            born = bo;

        }
        public void setName(string n)
        {
            name = n;
        }
        public string getName()
        {
            return name;
        }
        public void setWeight(float w)
        {
            weight = w;
        }
        public float getWeight()
        {
            return weight;
        }
        public void setHigh(float h)
        {
            high = h;
        }
        public float getHigh()
        {
            return high;
        }
        public void setAge(int a)
        {
            age = a;
        }
        public int getAge()
        {
            return age;
        }
        public float Imc()
        {
            float IMC = weight / (high * high);
            return IMC;
        }
        public void setNasc(Data bo)
        {
            born = bo;
        }
        public Data getNasc()
        {
            return born;
        }
        public int Diferenca(Pessoa outra)
        {
            int diferenca = outra.getNasc().getDiaAtual() - born.getDiaAtual();
            return diferenca;
        }
    }
    class Carro
    {
        private string marca;
        private string modelo;
        private string nome;
        private string cor;
        private string placa;
        private int portas;

        public Carro(string ma, string mo, string no, string co, string pl, int po)
        {
            marca = ma;
            modelo = mo;
            nome = no;
            cor = co;
            placa = pl;
            portas = po;
        }
        public void setMarca(string ma)
        {
            marca = ma;
        }
        public string getMarca()
        {
            return marca;
        }
        public void setModelo(string mo)
        {
            modelo = mo;
        }
        public string getModelo()
        {
            return modelo;
        }
        public void setNome(string no)
        {
            nome = no;
        }
        public string getNome()
        {
            return nome;
        }
        public void setCor(string co)
        {
            cor = co;
        }
        public string getCor()
        {
            return cor;
        }
        public void setPlaca(string pl)
        {
            placa = pl;
        }
        public string getPlaca()
        {
            return placa;
        }
        public void setPorta(int po)
        {
            portas = po;
        }
        public int getPorta()
        {
            return portas;
        }

    }
    class Data
    {
        private int ano;
        private int mes;
        private int dia;
        private bool b6;

        public Data(int an, int me, int di)
        {
            ano = an;
            mes = me;
            dia = di;

            if ((an % 4 == 0 && an % 100 != 0) || an % 400 == 0)
            {
                b6 = true;
            }
            else
            {
                b6 = false;
            }
        }
        public void setAno(int an)
        {
            ano = an;
        }
        public int getAno()
        {
            return ano;
        }
        public void setMes(int me)
        {
            mes = me;
        }
        public int getMes()
        {
            return mes;
        }
        public void setDia(int di)
        {
            dia = di;
        }
        public int getDia()
        {
            return dia;
        }
        public string getBx()
        {
            if (b6)
            {
                return "O ano é bissexeto";
            }
            else
            {
                return "Não é bissexto";
            }
        }


        public int getDiaAtual()
        {
            int cMes = 0;

            switch (mes)
            {
                case 1:
                case 3:
                case 5:
                case 7:
                case 8:
                case 10:
                case 12:
                    cMes = mes * 31;
                    break;

                case 4:
                case 6:
                case 9:
                case 11:
                    cMes = mes * 30;
                    break;

                case 2:
                    cMes = mes * 28;
                    break;

            }
            int cAno = ano * 365;
            int cDia = dia;
            int totDias = cAno + cMes + cDia;
            if (b6 == true)
            {
                totDias += 1;
                return totDias;
            }
            else
            {
                return totDias;
            }
        }


        public override string ToString()
        {
            return dia + "/" + mes + "/" + ano;
        }

        public string IncrementaUmDia()
        {
            dia++;
            if (dia > QuantDia())
            {
                dia = 1;
                mes++;
                if (mes > 12)
                {
                    mes = 1;
                    ano++;
                }
            }
            return dia + "/" + mes + "/" + ano;

        }
        public int QuantDia()
        {
            int qtdDia = 0;
            switch (mes)
            {
                case 1:
                case 3:
                case 5:
                case 7:
                case 8:
                case 10:
                case 12:
                     qtdDia = 31;
                break;

                case 4:
                case 6:
                case 9:
                case 11:
                    qtdDia = 30;
                    break;

                case 2:
                    if (b6)
                    {
                        qtdDia = 29;
                    }
                    else
                    {
                        qtdDia = 28;
                    }

                    break;
            }
            return qtdDia;
        }

    }
    class Produto
    {
        private string dataValidade;
        private string dataFabricacao;
        private string descricao;
        private float peso;
        private float preco;

        public Produto(string dv, string df, string ds, float pe, float pr)
        {
            dataValidade = dv;
            dataFabricacao = df;
            descricao = ds;
            peso = pe;
            preco = pr;
        }
        public void setData_v(string dv)
        {
            dataValidade = dv;
        }
        public string getData_v()
        {
            return dataValidade;
        }
        public void setData_f(string df)
        {
            dataFabricacao = df;
        }
        public string getData_f()
        {
            return dataFabricacao;
        }
        public void setDescricao(string ds)
        {
            descricao = ds;
        }
        public string getDescricao()
        {
            return descricao;
        }
        public void setPeso(float pe)
        {
            peso = pe;
        }
        public float getPeso()
        {
            return peso;
        }
        public void setPreco(float pr)
        {
            preco = pr;
        }
        public float getPreco()
        {
            return preco;
        }
        public string getAll()
        {
            string all = dataFabricacao + dataValidade + descricao + peso.ToString() + preco.ToString();
            return all;
        }
    }
    class Program
    {
        static void Main(string[] args)
        {

            // Pessoa someone = new Pessoa("Heisenberg", 85.5f, 1.97f, 29, new Data(2018, 01, 01));

            // Console.WriteLine("Nome: {0} - Peso {1} - Altura {2} - Idade {3} - Nascimento {4}", someone.getName(), someone.getWeight(), someone.getHigh(), someone.getAge(), someone.getNasc());

            //// Console.WriteLine("IMC da Pessoa: {0}", someone.Imc());

            // Carro veiculo = new Carro("Chevrolet", "Super Sport", "Opala", "Preto", "irn - 666", 2);

            // //Console.WriteLine("O carro da pessoa {0} é o {1}", someone.getName(), veiculo.getNome());

            // Data data = new Data(2000, 01, 01);

            //// Console.WriteLine("O ano é bissxesto? {0}", data.getBx());

            // Produto produto = new Produto("01/01/2018", "02/01/2018", "askljdfasdhfbakjdhb", 85.5f, 65.5f);

            // //Console.WriteLine("{0}", produto.getAll());

            //Data anterior = new Data(2017, 12, 31);
            //Data hoje = new Data(2018, 12, 31);
            //Console.WriteLine("{0}", hoje.getDiaAtual() - anterior.getDiaAtual());

            Data TESTE = new Data(2016, 02, 28);
            Pessoa someone = new Pessoa("Ragnar", 85.5f, 1.97f, 29, new Data(2018, 01, 01));
            Pessoa anyone = new Pessoa("Heisenberg", 85.5f, 1.97f, 29, new Data(2018, 01, 25));

            Console.WriteLine("{0}/{1}/{2}", TESTE.getDia(), TESTE.getMes(), TESTE.getAno());


            TESTE.IncrementaUmDia();


            Console.WriteLine("{0}/{1}/{2}", TESTE.getDia(), TESTE.getMes(), TESTE.getAno());


            Console.WriteLine("{0}", someone.Diferenca(anyone));



            Console.ReadKey();


        }
    }
}
