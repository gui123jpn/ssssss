<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elden Ring Fan Page</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root {
            --primary-color: #5e2e1d;
            --secondary-color: #a67c52;
            --accent-color: #d4a373;
            --dark-color: #1a1a1a;
            --light-color: #f8f9fa;
        }

        .dark-theme {
            --primary-color: #1a1a1a;
            --secondary-color: #333;
            --accent-color: #5e2e1d;
            --dark-color: #f8f9fa;
            --light-color: #1a1a1a;
        }

        body {
            font-family: 'Georgia', serif;
            background-color: var(--light-color);
            color: var(--dark-color);
            transition: all 0.3s ease;
        }

        .bg-custom {
            background-color: var(--primary-color);
        }

        .text-custom {
            color: var(--accent-color);
        }

        .border-custom {
            border-color: var(--secondary-color);
        }

        .game-card {
            background: linear-gradient(to bottom right, var(--secondary-color), var(--primary-color));
            box-shadow: 0 10px 20px rgba(0,0,0,0.3);
        }

        .music-player {
            background: rgba(0,0,0,0.7);
            backdrop-filter: blur(10px);
        }

        .tab.active {
            border-bottom: 3px solid var(--accent-color);
        }

        .comment-section {
            max-height: 400px;
            overflow-y: auto;
        }

        /* Scrollbar styling */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--secondary-color);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--accent-color);
            border-radius: 4px;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .flex-col-mobile {
                flex-direction: column;
            }
            
            .w-full-mobile {
                width: 100% !important;
            }
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Navigation -->
    <nav class="bg-custom text-white p-4 shadow-lg">
        <div class="container mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/171be1ce-0705-4bfa-a3d6-8f01c57df819.png" alt="Logo de Elden Ring mostrando o anel partido em dourado com fundo preto" class="h-10">
                <span class="text-xl font-bold">Elden Ring Fan Page</span>
            </div>
            <div class="flex space-x-4">
                <button id="themeToggle" class="px-4 py-2 bg-amber-700 hover:bg-amber-600 rounded transition">
                    Modo Escuro
                </button>
                <a href="#game-info" class="hover:text-amber-300 transition">Jogo</a>
                <a href="#character" class="hover:text-amber-300 transition">Personagem</a>
                <a href="#community" class="hover:text-amber-300 transition">Comunidade</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="relative h-96 flex items-center justify-center bg-black overflow-hidden">
        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/816385fc-a18c-40cb-b692-bf59474078d1.png" alt="Vista panorâmica da The Lands Between mostrando a Erdtree no horizonte com céu crepuscular" class="absolute w-full h-full object-cover opacity-70">
        <div class="relative z-10 text-center px-4">
            <h1 class="text-5xl md:text-6xl font-bold text-white mb-4">ELDEN RING</h1>
            <p class="text-xl text-amber-200 mb-8 max-w-2xl mx-auto">Torne-se o Lorde das Cinzas em uma jornada épica através das Terras Intermédias</p>
            <button class="px-6 py-3 bg-amber-700 hover:bg-amber-600 text-white rounded-full font-bold transition transform hover:scale-105">
                Explorar o Mundo
            </button>
        </div>
    </header>

    <div class="container mx-auto px-4 py-8">
        <!-- Game Information Section -->
        <section id="game-info" class="mb-16">
            <h2 class="text-3xl font-bold text-custom mb-6 border-b border-custom pb-2">Sobre o Jogo</h2>
            
            <div class="game-card rounded-lg p-6 text-white mb-8">
                <div class="flex flex-col md:flex-row gap-8">
                    <div class="md:w-1/2">
                        <h3 class="text-2xl font-bold mb-4">A Nova Obra-Prima da FromSoftware</h3>
                        <p class="mb-4">Elden Ring é um RPG de ação em mundo aberto desenvolvido pela FromSoftware em colaboração com George R.R. Martin, autor de "As Crônicas de Gelo e Fogo". Situado nas Terras Intermédias, o jogo combina a jogabilidade desafiadora característica dos jogos Souls com um vasto mundo para explorar.</p>
                        <p>Como um Maculado, você deve viajar pelo reino, derrotar demigodos e seus seguidores, e reunir os fragmentos do Elden Ring para se tornar o novo Lorde das Cinzas.</p>
                    </div>
                    <div class="md:w-1/2">
                        <div class="bg-black rounded-lg overflow-hidden">
                            <iframe class="w-full aspect-video" src="https://www.youtube.com/embed/E3Huy2cdih0" title="Trailer de Elden Ring" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                    </div>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <div class="text-amber-600 text-3xl mb-3">🌎</div>
                    <h3 class="text-xl font-bold mb-2">Mundo Aberto</h3>
                    <p>Explore um mundo vasto e interconectado cheio de segredos, masmorras e inimigos desafiadores.</p>
                </div>
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <div class="text-amber-600 text-3xl mb-3">⚔️</div>
                    <h3 class="text-xl font-bold mb-2">Combate Intenso</h3>
                    <p>Sistema de combate profundo com diversas armas, magias e habilidades para dominar.</p>
                </div>
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <div class="text-amber-600 text-3xl mb-3">🧩</div>
                    <h3 class="text-xl font-bold mb-2">História Enigmática</h3>
                    <p>Narrativa fragmentada que encoraja a exploração e interpretação do jogador.</p>
                </div>
            </div>
        </section>

        <!-- Character Section -->
        <section id="character" class="mb-16">
            <h2 class="text-3xl font-bold text-custom mb-6 border-b border-custom pb-2">Meu Personagem</h2>
            
            <div class="flex flex-col md:flex-row gap-8 items-center md:items-start">
                <div class="w-full md:w-1/3">
                    <div class="relative group">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/7f34a14e-cac7-418b-a9b6-22ebd020ea38.png" alt="Personagem personalizado Tarnished usando armadura de Cavaleiro de Caria, empunhando a espada Moonveil com magias lunares brilhando ao redor em um campo de flores" class="w-full rounded-lg shadow-xl transform group-hover:scale-105 transition duration-300">
                        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100 flex items-center justify-center transition duration-300 rounded-lg">
                            <span class="text-white font-bold">Tarnished - Nível 125</span>
                        </div>
                    </div>
                    
                    <div class="mt-4 text-center">
                        <h3 class="text-2xl font-bold">Astrologer Renato</h3>
                        <p class="text-sm text-gray-600 dark:text-gray-300">Maculado da Lua</p>
                        
                        <div class="mt-4 flex justify-center space-x-2">
                            <span class="px-3 py-1 bg-blue-100 dark:bg-blue-900 text-blue-800 dark:text-blue-200 rounded-full text-xs">Inteligência</span>
                            <span class="px-3 py-1 bg-purple-100 dark:bg-purple-900 text-purple-800 dark:text-purple-200 rounded-full text-xs">Magia</span>
                            <span class="px-3 py-1 bg-gray-100 dark:bg-gray-900 text-gray-800 dark:text-gray-200 rounded-full text-xs">Agilidade</span>
                        </div>
                    </div>
                </div>
                
                <div class="w-full md:w-2/3">
                    <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6 h-full">
                        <h3 class="text-xl font-bold mb-4 text-custom">Build Details</h3>
                        
                        <div class="grid grid-cols-2 gap-4 mb-6">
                            <div>
                                <h4 class="font-semibold">Arma Primária</h4>
                                <p>Moonveil Katana +10</p>
                            </div>
                            <div>
                                <h4 class="font-semibold">Escudo</h4>
                                <p>Carian Shield +8</p>
                            </div>
                            <div>
                                <h4 class="font-semibold">Armadura</h4>
                                <p>Conjunto Carian Knight</p>
                            </div>
                            <div>
                                <h4 class="font-semibold">Talismãs</h4>
                                <p>Graven-Mass, Radagon Icon, Dragoncrest, Moon of Nokstella</p>
                            </div>
                        </div>
                        
                        <h4 class="font-semibold mb-2 text-custom">Descrição do Build</h4>
                        <p class="mb-4">Este build foca no uso da Moonveil Katana combinada com magias de gelo e lunar. Uma abordagem equilibrada entre combate corpo-a-corpo e magia de longa distância, ideal para duelos PvP e contra chefes.</p>
                        
                        <h4 class="font-semibold mb-2 text-custom">Magias Principais</h4>
                        <ul class="list-disc pl-5 mb-4">
                            <li>Adula's Moonblade</li>
                            <li>Stars of Ruin</li>
                            <li>Glintstone Icecrag</li>
                            <li>Terra Magica</li>
                        </ul>
                        
                        <div class="music-player p-4 rounded-lg mt-6">
                            <h4 class="font-bold text-white mb-3">Trilha Sonora</h4>
                            <div class="flex items-center space-x-4">
                                <button id="playBtn" class="bg-amber-600 hover:bg-amber-500 text-white rounded-full w-10 h-10 flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z" clip-rule="evenodd" />
                                    </svg>
                                </button>
                                <button id="pauseBtn" class="bg-amber-600 hover:bg-amber-500 text-white rounded-full w-10 h-10 flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                                        <path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zM7 8a1 1 0 012 0v4a1 1 0 11-2 0V8zm5-1a1 1 0 00-1 1v4a1 1 0 102 0V8a1 1 0 00-1-1z" clip-rule="evenodd" />
                                    </svg>
                                </button>
                                <button id="stopBtn" class="bg-amber-600 hover:bg-amber-500 text-white rounded-full w-10 h-10 flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                                        <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM8 7a1 1 0 00-1 1v4a1 1 0 001 1h4a1 1 0 001-1V8a1 1 0 00-1-1H8z" clip-rule="evenodd" />
                                    </svg>
                                </button>
                                <span class="text-white">"The Final Battle" - Elden Ring OST</span>
                            </div>
                            <audio id="gameMusic" loop>
                                <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
                            </audio>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="mt-8">
                <h3 class="text-2xl font-bold text-custom mb-4">Minha Jornada</h3>
                <p class="mb-4">Comecei como um astrologer modesto, usando apenas um bastão e magias básicas. Ao explorar as Terras Intermédias, descobri a Moonveil Katana nas minas de Gael e desde então desenvolvi este build híbrido único que combina a agressividade de uma katana com o poder das magias lunares.</p>
                <p>Minha maior conquista foi derrotar Malenia, Blade of Miquella, após 87 tentativas. Essa vitória marcou minha transformação de um simples mago para um verdadeiro Cavaleiro da Lua.</p>
            </div>
        </section>

        <!-- Community Section -->
        <section id="community" class="mb-16">
            <h2 class="text-3xl font-bold text-custom mb-6 border-b border-custom pb-2">Comunidade</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Tips and Tricks -->
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <h3 class="text-xl font-bold mb-4 text-custom">Dicas e Truques</h3>
                    
                    <div class="space-y-4">
                        <div class="p-4 border border-amber-200 rounded-lg">
                            <h4 class="font-semibold text-amber-700 dark:text-amber-300">Contra Malenia</h4>
                            <p class="text-sm">Use a habilidade "Transient Moonlight" da Moonveil para interromper seus ataques a distância. Traga summons que causem sangramento como Mimic Tear ou Tiche.</p>
                        </div>
                        
                        <div class="p-4 border border-amber-200 rounded-lg">
                            <h4 class="font-semibold text-amber-700 dark:text-amber-300">Fazenda de Runes</h4>
                            <p class="text-sm">Na área de Mohgwyn Palace, há um local com muitos Albinaurics que dão 50k runes por corrida com o Gold Scarab Talisman.</p>
                        </div>
                        
                        <div class="p-4 border border-amber-200 rounded-lg">
                            <h4 class="font-semibold text-amber-700 dark:text-amber-300">Segredos Ocultos</h4>
                            <p class="text-sm">No subterrâneo de Leyndell há uma passagem secreta que leva a um conjunto de armadura exclusivo. Use ataques rolantes para revelar paredes ilusórias.</p>
                        </div>
                    </div>
                </div>
                
                <!-- Comments Section -->
                <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg p-6">
                    <h3 class="text-xl font-bold mb-4 text-custom">Comentários da Comunidade</h3>
                    
                   
