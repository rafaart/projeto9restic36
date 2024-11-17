# projeto9restic36

"cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/rafaart/projeto9restic36/blob/develop/AVALIA%C3%87%C3%83O_9_RegLinear.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "fBsTbbixyd1V"
      },
      "source": [
        "## YURI OLIVEIRA DOS SANTOS e RAFAEL SANTOS SOUZA"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "FM4RpCectZEq"
      },
      "source": [
        "# Projeto: Implementação e Análise do Algoritmo de Regressão Linear\n",
        "\n",
        "# Sobre a base de dados🎲\n",
        "Este conjunto de dados reúne informações sobre os principais influenciadores do Instagram, abrangendo uma variedade de 200 tipos diferentes de influenciadores. Ele inclui perfis com grande número de seguidores, alto engajamento e amplo alcance em suas postagens.\n",
        "\n",
        "\n",
        "# Uso da base: 🛠️\n",
        "\n",
        "O conjunto de dados pode ser usado para:\n",
        "\n",
        "Esse tipo de conjunto de dados é usado para entender tendências nas mídias sociais, analisar o comportamento dos influenciadores e ajudar marcas a identificar os perfis mais adequados para campanhas de marketing.\n",
        "\n",
        "# Objetivo do nosso projeto:🎯\n",
        "\n",
        "Este notebook contempla a criação de um modelo preditivo usando o algoritmo de Regressão Linear para resolver um problema de inferência sobre taxa de engajamento dos principais influenciadores do instagram \"Top Instagram Influencers Data\" do Kaggle.\n",
        "\n",
        "O link desta base e mais detalhes se encontra em: https://www.kaggle.com/datasets/surajjha101/top-instagram-influencers-data-cleaned"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "h-WbxhTWD2MT"
      },
      "source": [
        "# <h1 style='background:#00FFFF; border:2; border-radius: 10px; font-size:250%; font-weight: bold; color:black'><center>TOP INSTAGRAM INFLUENCERS DATA</center></h1>\n",
        "\n",
        "<img src = \"https://i.gifer.com/9uhG.gif\" width = 900 height = 400/>\n",
        "\n",
        "Sobre este arquivo:\n",
        "\n",
        "Neste arquivo, basicamente há 10 atributos. Ele foi ordenado com base na classificação que foi decidida com base em \"seguidores\".\n",
        "\n",
        "rank: Classificação do Influenciador com base no número de seguidores que ele tem\n",
        "\n",
        "channel_info: Nome de usuário do Instagrammer\n",
        "\n",
        "influence score: Pontuação de influência dos usuários. É calculado com base em menções, importância e popularidade\n",
        "\n",
        "posts: Número de posts que eles fizeram até agora\n",
        "\n",
        "followers: Número de seguidores do usuário\n",
        "\n",
        "avg_likes: Média de curtidas em posts do Instagrammer (total de curtidas/total de posts)\n",
        "\n",
        "60_day_eng_rate: Taxa de engajamento dos últimos 60 dias do Instagrammer como facção de engajamentos que eles fizeram até agora\n",
        "\n",
        "new_post_avg_like: Média de curtidas que eles têm em novos posts\n",
        "\n",
        "total de curtidas: Total de curtidas que o usuário obteve em seus posts. (em bilhões)\n",
        "\n",
        "country: País ou região de origem do usuário.\n",
        "<a id='top'></a>\n",
        "<div class=\"list-group\" id=\"list-tab\" role=\"tablist\">\n",
        "    "
      ]
    },
