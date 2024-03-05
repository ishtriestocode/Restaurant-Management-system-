{
  "cells": [
    {
      "cell_type": "code",
      "execution_count": null,
      "id": "bc37d300",
      "metadata": {
        "id": "bc37d300"
      },
      "outputs": [],
      "source": [
        "class PythonCafeTalk:\n",
        "    def restaurants(rp):\n",
        "        print(\"\\t\\t\\t\\t Python Cafe Talk\")\n", 
        "        print(\"\\t\\t\\t\\t Since-1997\")\n",
        "        print(\"\\t\\t\\t\\t www.fuddybuddy.com\")\n",
        "        print(\"\\n\\n\\t\\t\\t\\t\\tMENU\")\n",
        "\n",
        "    def food(rp):\n",
        "        x=[\"Indian\",\"German\",\"Korean\",\"Vietnamese\"]\n",
        "        for k in x:\n",
        "            print(\"\\n\\n\",k)\n",
        "\n",
        "    def german(rp):\n",
        "        x=[\"Sauerbraten-roas beef stew \",\"Schweinshaxe-pork knuckle\",\"Rinderroulade-beef roll\",\"Bratwurst-grilled sausage\",\"Kartoffelpuffer-potato pancake\",\"Kartoffelkloesse-potato dumplings\",\"Sauerkraut-fermented cabbage\",\"Spatzle-Egg noodles\"]\n",
        "        y=[250,300,150,100,200,100,350,180]\n",
        "        german_={\"German Food Types\":x,\"Price\":y}\n",
        "        import pandas as pd\n",
        "        df=pd.DataFrame(german_)\n",
        "        print(\"\\n\\n German Foods \\n\\n\")\n",
        "        print(df)\n",
        "        d=[]\n",
        "        while x:\n",
        "            x=True\n",
        "            b=int(input(\"Enter the value position : \"))\n",
        "            c=int(input(\"Enter the Quantity:\"))\n",
        "            z=german_[\"Price\"][b]\n",
        "            y=z*c\n",
        "            d.append(y)\n",
        "            x=input(\"you want to reorder(yes/no):\")\n",
        "            if(x==\"no\"):\n",
        "                print('Thank you')\n",
        "                break\n",
        "        t=sum(d)\n",
        "        m=(sum(d)*0.05)\n",
        "        k=t+m\n",
        "        print(\"servicetax = 5%\")\n",
        "        print(\"Total Amount:\",t,\"Rupees\")\n",
        "        print(\"Total Amount Including Service Tax:\",k,\"Rupees\")\n",
        "\n",
        "\n",
        "    def korean(rp):\n",
        "        x=[\"Kimchi\",\"Bibimbap\",\"Bulgogi\",\"Jajangmyeon\",\"Samgyeopsal\",\"Korean fried chicken\",\"Red rice cakes - tteokbokki\"]\n",
        "        y=[200,100,350,400,100,345,250]\n",
        "        korean_={\"Korean Food Types\":x,\"Price\":y}\n",
        "        import pandas as pd\n",
        "        df=pd.DataFrame(korean_)\n",
        "        print(\"\\n\\n Korean Foods \\n\\n\")\n",
        "        print(df)\n",
        "        d=[]\n",
        "        while x:\n",
        "            x=True\n",
        "            b=int(input(\"Enter the value position : \"))\n",
        "            c=int(input(\"Enter the Quantity:\"))\n",
        "            z=korean_[\"Price\"][b]\n",
        "            y=z*c\n",
        "            d.append(y)\n",
        "            x=input(\"you want to reorder(yes/no):\")\n",
        "            if(x==\"no\"):\n",
        "                print('Thank you')\n",
        "                break\n",
        "        t=sum(d)\n",
        "        m=(sum(d)*0.05)\n",
        "        k=t+m\n",
        "        print(\"servicetax = 5%\")\n",
        "        print(\"Total Amount:\",t,\"Rupees\")\n",
        "        print(\"Total Amount Including Service Tax:\",k,\"Rupees\")\n",
        "\n",
        "\n",
        "\n",
        "\n",
        "    def vietnamese(rp):\n",
        "        x=[\"Pho\",\"Bun cha\",\"Banh mi\",\"Banh cuon\",\"Goi cuon\"]\n",
        "        y=[250,300,200,100,500]\n",
        "        vietnamese_={\"Vietnamese Food Types\":x,\"Price\":y}\n",
        "        import pandas as pd\n",
        "        df=pd.DataFrame(vietnamese_)\n",
        "        print(\"\\n\\n Vietnamese Foods \\n\\n\")\n",
        "        print(df)\n",
        "        d=[]\n",
        "        while x:\n",
        "            x=True\n",
        "            b=int(input(\"Enter the value position : \"))\n",
        "            c=int(input(\"Enter the Quantity:\"))\n",
        "            z=vietnamese_[\"Price\"][b]\n",
        "            y=z*c\n",
        "            d.append(y)\n",
        "            x=input(\"you want to reorder(yes/no):\")\n",
        "            if(x==\"no\"):\n",
        "                print('Thank you')\n",
        "                break\n",
        "        t=sum(d)\n",
        "        m=(sum(d)*0.05)\n",
        "        k=t+m\n",
        "        print(\"servicetax = 5%\")\n",
        "        print(\"Total Amount:\",t,\"Rupees\")\n",
        "        print(\"Total Amount Including Service Tax:\",k,\"Rupees\")\n",
        "\n",
        "\n",
        "\n",
        "    def indian(rp):\n",
        "        x=[\"Misal Pav\",\"Kosha Mangsho\",\"Makki Di Roti& sarso da saag\",\"Dhokla\",\"Rogan Josh\",\"Papaya Khar\",\"Litti Chowkha\",\"Biryani\",\"Fish Curry\"]\n",
        "        y=[80,200,350,120,200,150,250,400,500]\n",
        "        indian_={\"Indian Food Types\":x,\"Price\":y}\n",
        "        import pandas as pd\n",
        "        df=pd.DataFrame(indian_)\n",
        "        print(\"\\n\\n Indian Foods \\n\\n\")\n",
        "        print(df)\n",
        "        d=[]\n",
        "        while x:\n",
        "            x=True\n",
        "            b=int(input(\"Enter the value position : \"))\n",
        "            c=int(input(\"Enter the Quantity:\"))\n",
        "            z=indian_[\"Price\"][b]\n",
        "            y=z*c\n",
        "            d.append(y)\n",
        "            x=input(\"you want to reorder(yes/no):\")\n",
        "            if(x==\"no\"):\n",
        "                print('Thank you')\n",
        "                break\n",
        "        t=sum(d)\n",
        "        m=(sum(d)*0.05)\n",
        "        k=t+m\n",
        "        from colorama import Fore,Back,Style\n",
        "        print(Fore.BLACK+Back.RED+Style.BRIGHT+\"servicetax = 5%\")\n",
        "        print(\"Total Amount:\",t,\"Rupees\")\n",
        "        print(\"Total Amount Including Service Tax:\",k,\"Rupees\")\n",
        ""
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "id": "65707c68",
      "metadata": {
        "id": "65707c68",
        "outputId": "fc152b00-dcf7-485b-974f-2bfe0cb2e714"
      },
      "outputs": [
        {
          "name": "stdout",
          "output_type": "stream",
          "text": [
            "\t\t\t\t Python Cafe Talk\n",
            "\t\t\t\t Since-1997\n",
            "\t\t\t\t www.fuddybuddy.com\n",
            "\n",
            "\n",
            "\t\t\t\t\tMENU\n",
            "\n",
            "\n",
            " Indian\n",
            "\n",
            "\n",
            " German\n",
            "\n",
            "\n",
            " Korean\n",
            "\n",
            "\n",
            " Vietnamese\n"
          ]
        }
      ],
      "source": [
        "obj=PythonCafeTalk()\n",
        "obj.restaurants()\n",
        "obj.food()\n"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "id": "b2ea7994",
      "metadata": {
        "id": "b2ea7994",
        "outputId": "3f94c372-657a-4266-8a48-570eb5f52a32"
      },
      "outputs": [
        {
          "name": "stdout",
          "output_type": "stream",
          "text": [
            "Enter the Type of food : indian\n",
            "\n",
            "\n",
            " Indian Foods \n",
            "\n",
            "\n",
            "              Indian Food Types  Price\n",
            "0                     Misal Pav     80\n",
            "1                 Kosha Mangsho    200\n",
            "2  Makki Di Roti& sarso da saag    350\n",
            "3                        Dhokla    120\n",
            "4                    Rogan Josh    200\n",
            "5                   Papaya Khar    150\n",
            "6                 Litti Chowkha    250\n",
            "7                       Biryani    400\n",
            "8                    Fish Curry    500\n",
            "Enter the value position : 7\n",
            "Enter the Quantity:4\n",
            "you want to reorder(yes/no):yes\n",
            "Enter the value position : 3\n",
            "Enter the Quantity:2\n",
            "you want to reorder(yes/no):yes\n",
            "Enter the value position : 8\n",
            "Enter the Quantity:2\n",
            "you want to reorder(yes/no):no\n",
            "Thank you\n",
            "\u001b[30m\u001b[41m\u001b[1mservicetax = 5%\n",
            "Total Amount: 2840 Rupees\n",
            "Total Amount Including Service Tax: 2982.0 Rupees\n",
            "None\n"
          ]
        }
      ],
      "source": [
        "x=input(\"Enter the Type of food : \")\n",
        "if x==\"indian\":\n",
        "    print(obj.indian())\n",
        "elif x==\"german\":\n",
        "    print(obj.german())\n",
        "elif x==\"korean\":\n",
        "    print(obj.korean())\n",
        "elif x==\"vietnamese\":\n",
        "    print(obj.vietnamese())\n",
        "else:\n",
        "    print(\"wrong option: \\nplease again choose the right option:\")"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "id": "1bba9de7",
      "metadata": {
        "id": "1bba9de7"
      },
      "outputs": [],
      "source": [
        "class PythonCafeTalk:\n",
        "    def __init__(rp):\n",
        "        print(\"\\t\\t\\t\\t Python Cafe Talk\")\n",
        "        print(\"\\t\\t\\t\\t Since-1997\")\n",
        "        print(\"\\t\\t\\t\\t www.fuddybuddy.com\")\n",
        "        print(\"\\n\\n\\t\\t\\t\\t\\tMENU\")\n",
        "\n",
        "        x=[\"Indian\",\"German\",\"Korean\",\"Vietnamese\"]\n",
        "        for k in x:\n",
        "            print(\"\\n\\n\",k)"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "id": "363930d1",
      "metadata": {
        "id": "363930d1",
        "outputId": "855ea659-a15a-486e-98a6-6fbd42ba14c0"
      },
      "outputs": [
        {
          "name": "stdout",
          "output_type": "stream",
          "text": [
            "\t\t\t\t Python Cafe Talk\n",
            "\t\t\t\t Since-1997\n",
            "\t\t\t\t www.fuddybuddy.com\n",
            "\n",
            "\n",
            "\t\t\t\t\tMENU\n",
            "\n",
            "\n",
            " Indian\n",
            "\n",
            "\n",
            " German\n",
            "\n",
            "\n",
            " Korean\n",
            "\n",
            "\n",
            " Vietnamese\n"
          ]
        }
      ],
      "source": [
        "obj=PythonCafeTalk()\n"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "id": "4db06017",
      "metadata": {
        "id": "4db06017"
      },
      "outputs": [],
      "source": []
    }
  ],
  "metadata": {
    "kernelspec": {
      "display_name": "Python 3 (ipykernel)",
      "language": "python",
      "name": "python3"
    },
    "language_info": {
      "codemirror_mode": {
        "name": "ipython",
        "version": 3
      },
      "file_extension": ".py",
      "mimetype": "text/x-python",
      "name": "python",
      "nbconvert_exporter": "python",
      "pygments_lexer": "ipython3",
      "version": "3.9.7"
    },
    "colab": {
      "provenance": []
    }
  },
  "nbformat": 4,
  "nbformat_minor": 5
}
