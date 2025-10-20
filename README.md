<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brownie Simples - A Receita Perfeita</title>
    <!-- Inclui o Tailwind CSS para estilização rápida e responsiva -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Define a fonte padrão como Inter (ou fallback sans-serif) e cores de fundo */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f3f0; /* Um off-white suave */
            color: #333;
        }
        /* Cor de destaque para botões e cabeçalhos menores - marrom chocolate */
        .color-primary {
            color: #5d4037;
        }
        .bg-primary {
            background-color: #5d4037;
        }
        /* Estilo para a imagem de fundo/banner, escurecendo para melhor contraste do texto */
        .hero-bg {
            background-image: url('https://placehold.co/1200x600/6D4C41/FFFFFF?text=Brownie+Delicioso');
            background-size: cover;
            background-position: center;
        }
        /* Estilo para a caixa da receita - elevando-a visualmente */
        .recipe-box {
            background-color: #ffffff;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        /* Estilo para a seção de ingredientes (melhora a visibilidade da lista) */
        ul.ingredients-list li {
            position: relative;
            padding-left: 1.5rem;
            margin-bottom: 0.5rem;
        }
        ul.ingredients-list li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: #8d6e63; /* Marrom mais claro para o ponto */
            font-weight: bold;
        }
    </style>
</head>
<body>

    <!-- Cabeçalho Simples -->
    <header class="p-4 bg-white shadow-md">
        <div class="max-w-6xl mx-auto flex justify-between items-center">
            <h1 class="text-3xl font-bold color-primary tracking-tight">
                Brownie Simples
            </h1>
            <nav>
                <a href="#receita" class="text-gray-600 hover:color-primary transition duration-300">A Receita</a>
                <a href="#" class="ml-4 text-gray-600 hover:color-primary transition duration-300 hidden sm:inline">Variações</a>
            </nav>
        </div>
    </header>

    <!-- Seção Hero/Destaque -->
    <section class="hero-bg h-96 flex items-center justify-center text-white text-center rounded-b-xl mb-12">
        <div class="p-6 bg-black bg-opacity-40 rounded-xl max-w-lg">
            <h2 class="text-4xl sm:text-5xl font-extrabold mb-4">O Brownie Perfeito</h2>
            <p class="text-lg mb-6">Fudgy, crocante por cima e irresistivelmente simples de fazer.</p>
            <a href="#receita" class="inline-block px-8 py-3 bg-orange-600 text-white font-semibold rounded-full hover:bg-orange-700 transition duration-300 shadow-lg">
                Começar a Fazer
            </a>
        </div>
    </section>

    <!-- Container Principal da Receita -->
    <main id="receita" class="max-w-5xl mx-auto p-4 sm:p-6 lg:p-8">

        <!-- Informações Rápidas e Resumo -->
        <div class="recipe-box p-6 sm:p-8 rounded-xl mb-12">
            <h3 class="text-3xl font-bold color-primary mb-6 border-b-2 border-orange-200 pb-2">Receita Clássica de Brownie</h3>
            
            <!-- Ficha Técnica -->
            <div class="flex flex-wrap justify-around text-center mb-6 border-b pb-4">
                <div class="w-1/3 p-2">
                    <p class="text-lg font-bold text-gray-800">35 min</p>
                    <p class="text-sm text-gray-500">Preparo</p>
                </div>
                <div class="w-1/3 p-2 border-l border-r border-gray-200">
                    <p class="text-lg font-bold text-gray-800">25 min</p>
                    <p class="text-sm text-gray-500">Forno (180°C)</p>
                </div>
                <div class="w-1/3 p-2">
                    <p class="text-lg font-bold text-gray-800">16</p>
                    <p class="text-sm text-gray-500">Porções</p>
                </div>
            </div>

            <!-- Colunas de Ingredientes e Preparo (Layout Grid Responsivo) -->
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-10">
                
                <!-- Coluna 1: Ingredientes -->
                <div class="lg:col-span-1">
                    <h4 class="text-2xl font-semibold color-primary mb-4">Ingredientes</h4>
                    <ul class="ingredients-list list-none pl-0 text-lg">
                        <li>200g de chocolate meio amargo (picado)</li>
                        <li>150g de manteiga sem sal</li>
                        <li>1 xícara (200g) de açúcar cristal ou refinado</li>
                        <li>½ xícara (100g) de açúcar mascavo (opcional, mas recomendado)</li>
                        <li>3 ovos grandes</li>
                        <li>1 colher de chá de essência de baunilha</li>
                        <li>¾ xícara (90g) de farinha de trigo</li>
                        <li>¼ xícara (30g) de cacau em pó 100%</li>
                        <li>½ colher de chá de sal</li>
                        <li>½ xícara de nozes picadas ou gotas de chocolate (opcional)</li>
                    </ul>
                </div>

                <!-- Coluna 2 & 3: Modo de Preparo -->
                <div class="lg:col-span-2">
                    <h4 class="text-2xl font-semibold color-primary mb-4">Modo de Preparo</h4>
                    <ol class="space-y-6 text-gray-700">
                        <!-- Passo 1 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">1.</span>
                            Pré-aqueça o forno a 180°C. Unte e forre uma forma quadrada (aprox. 20x20cm) com papel manteiga, deixando sobras nas laterais para facilitar a remoção.
                        </li>
                        <!-- Passo 2 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">2.</span>
                            Em banho-maria ou no micro-ondas, derreta o chocolate meio amargo junto com a manteiga. Misture até ficar liso e reserve para esfriar um pouco.
                        </li>
                        <!-- Passo 3 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">3.</span>
                            Em uma tigela grande, bata ligeiramente os ovos com o açúcar cristal, o açúcar mascavo e a baunilha. Não precisa bater demais, apenas misturar.
                        </li>
                        <!-- Passo 4 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">4.</span>
                            Despeje a mistura de chocolate e manteiga derretidos sobre os ovos e misture delicadamente com um *fouet* ou espátula até incorporar.
                        </li>
                        <!-- Passo 5 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">5.</span>
                            Peneire a farinha de trigo, o cacau em pó e o sal sobre a mistura líquida. Dobre a massa (movimento de baixo para cima) apenas até que os ingredientes secos sumam. **Não misture demais!** (Isso garante o brownie *fudgy*).
                        </li>
                        <!-- Passo 6 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">6.</span>
                            Adicione as nozes ou gotas de chocolate (se usar) e despeje a massa na forma preparada.
                        </li>
                        <!-- Passo 7 -->
                        <li class="p-4 bg-gray-50 rounded-lg">
                            <span class="text-xl font-bold color-primary mr-2">7.</span>
                            Asse por 25 a 30 minutos. O topo deve estar firme e com rachaduras finas, mas o centro deve ainda parecer um pouco mole quando agitado. Retire do forno, deixe esfriar completamente na forma antes de cortar (idealmente, por 2 horas ou mais).
                        </li>
                    </ol>
                    
                    <!-- Dica Bônus -->
                    <div class="mt-8 p-4 bg-orange-100 border-l-4 border-orange-500 text-orange-800 rounded-md">
                        <p class="font-bold">Dica Secreta:</p>
                        <p class="text-sm">Para a casquinha perfeita, bata a mistura de ovos e açúcar até ficar um pouco mais clara antes de adicionar o chocolate derretido.</p>
                    </div>
                </div>
            </div>
        </div>

    </main>

    <!-- Rodapé Simples -->
    <footer class="mt-12 p-6 bg-primary text-white text-center">
        <p class="text-sm">&copy; 2025 Brownie Simples. Cozinhando com facilidade.</p>
        <p class="text-xs mt-2">Design minimalista com Tailwind CSS.</p>
    </footer>

</body>
</html>
