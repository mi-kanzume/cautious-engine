<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-title" content="🥜ィュ占い">
    <meta name="theme-color" content="#f59e0b">
    <meta name="description" content="毎日の運勢をピーナッツで占おう!">
    
    <title>🥜ィュ占い🥜</title>
    
    <!-- PWA Manifest -->
    <link rel="manifest" href="manifest.json">
    
    <!-- Apple Touch Icons -->
    <link rel="apple-touch-icon" href="icon-192.png">
    <link rel="apple-touch-icon" sizes="512x512" href="icon-512.png">
    
    <!-- Favicon -->
    <link rel="icon" type="image/png" href="icon-192.png">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- React -->
    <script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            -webkit-user-select: none;
            user-select: none;
            -webkit-tap-highlight-color: transparent;
            overscroll-behavior: none;
        }
        
        /* iOS用のスタイル調整 */
        @supports (-webkit-touch-callout: none) {
            body {
                min-height: -webkit-fill-available;
            }
        }
        
        /* インストールバナー非表示 */
        .pwa-install-prompt {
            display: none;
        }
    </style>
</head>
<body>
    <div id="root"></div>
    
    <script type="text/babel">
        const { useState } = React;
        const { Sparkles, Heart, Briefcase, Activity, Star } = lucide;

        function PeanutFortune() {
            const [cracked, setCracked] = useState(false);
            const [fortune, setFortune] = useState(null);
            const [shaking, setShaking] = useState(false);

            const fortunes = [
                {
                    type: '大吉',
                    color: 'from-yellow-400 to-orange-500',
                    overall: '殻を割ると、立派な双子の豆が!最高の一日になりそうです。',
                    love: 'ペアのピーナッツのように、素敵な出会いや絆の深まりが。💕',
                    work: '努力が実を結ぶ時。上司からの評価アップの予感!📈',
                    health: '体調絶好調!エネルギーに満ち溢れています。',
                    lucky: { color: 'ゴールド', item: 'ナッツミックス' }
                },
                {
                    type: '大吉',
                    color: 'from-yellow-400 to-orange-500',
                    overall: '完璧に熟したピーナッツ発見!幸運が次々と訪れる予感。',
                    love: '運命的な出会いがあるかも。直感を信じて!💘',
                    work: '大きなチャンスが舞い込む日。積極的に手を挙げて!',
                    health: 'パワー全開!新しいことにチャレンジする好機です。',
                    lucky: { color: 'サンライズオレンジ', item: 'ハニーナッツ' }
                },
                {
                    type: '中吉',
                    color: 'from-green-400 to-emerald-500',
                    overall: '新鮮なピーナッツの香り。穏やかで良い一日になりそう。',
                    love: '温かいコミュニケーションが幸せを運んでくれます。💝',
                    work: 'コツコツとした努力が認められる日。焦らず着実に。',
                    health: 'バランスの取れた食事を心がけて。特にナッツ類がおすすめ!',
                    lucky: { color: 'グリーン', item: 'ピーナッツバター' }
                },
                {
                    type: '中吉',
                    color: 'from-green-400 to-emerald-500',
                    overall: '香ばしく煎られたピーナッツのよう。充実した一日が待っています。',
                    love: '思いやりのある行動が、相手の心をぐっと掴みます。💚',
                    work: 'チームでの成功が期待できる日。協調性を大切に。',
                    health: '深呼吸とストレッチで、心身ともにリラックスを。',
                    lucky: { color: 'エメラルドグリーン', item: 'グリーンナッツ' }
                },
                {
                    type: '吉',
                    color: 'from-blue-400 to-cyan-500',
                    overall: '殻の中には可能性がいっぱい。小さな幸せを見つける日。',
                    love: '友人からの紹介や、何気ない会話から発展するかも。💌',
                    work: '新しいアイデアが浮かぶ日。メモを取っておくと吉。',
                    health: '適度な運動で心身ともにリフレッシュを。',
                    lucky: { color: 'スカイブルー', item: 'ペアのもの' }
                },
                {
                    type: '吉',
                    color: 'from-blue-400 to-cyan-500',
                    overall: 'カリッと割れる殻の音。爽やかな幸運が舞い込みます。',
                    love: '笑顔が鍵!明るい態度が良い縁を引き寄せます。😊',
                    work: '創造性が高まる日。柔軟な発想で問題解決を。',
                    health: '水分補給を忘れずに。清涼感のある飲み物がおすすめ。',
                    lucky: { color: 'ターコイズ', item: '塩味ナッツ' }
                },
                {
                    type: '吉',
                    color: 'from-indigo-400 to-blue-500',
                    overall: '丁寧に選別されたピーナッツ。質の高い一日になりそう。',
                    love: 'じっくりと関係を深める時期。焦らず自然体で。💙',
                    work: '専門性を活かせる場面が。あなたの知識が役立ちます。',
                    health: '規則正しい生活リズムを心がけて。質の良い睡眠を。',
                    lucky: { color: 'ミッドナイトブルー', item: 'カシューナッツ' }
                },
                {
                    type: '小吉',
                    color: 'from-pink-400 to-rose-500',
                    overall: '小さな幸運が転がっています。見逃さないように注意!',
                    love: '素直な気持ちを伝えることで、関係が一歩前進。💖',
                    work: '周りの人との協力が鍵。チームワークを大切に。',
                    health: '睡眠時間をしっかり確保して。休息も大事です。',
                    lucky: { color: 'ピンク', item: '小さなスナック' }
                },
                {
                    type: '小吉',
                    color: 'from-pink-400 to-rose-500',
                    overall: 'ひとつぶひとつぶに愛情を。小さな積み重ねが大切な日。',
                    love: 'さりげない優しさが、相手に届く日。気配りを忘れずに。🌸',
                    work: '細部にこだわることで、クオリティアップ!丁寧に。',
                    health: 'セルフケアの時間を大切に。好きな香りでリラックス。',
                    lucky: { color: 'さくらピンク', item: 'ストロベリーナッツ' }
                },
                {
                    type: '末吉',
                    color: 'from-purple-400 to-violet-500',
                    overall: 'ゆっくり殻を剥くように、焦らず丁寧に過ごす日。',
                    love: '相手のペースを尊重することで、信頼が深まります。💜',
                    work: '細かい確認作業が大切。ミスに注意して慎重に。',
                    health: 'ストレス解消に、好きなものを少し食べるのもあり。',
                    lucky: { color: 'ラベンダー', item: 'ローストピーナッツ' }
                },
                {
                    type: '末吉',
                    color: 'from-purple-400 to-violet-500',
                    overall: '熟成を待つピーナッツのよう。今は準備の時間です。',
                    love: '焦りは禁物。ゆっくりと信頼関係を築いていきましょう。🌙',
                    work: 'じっくり計画を練る日。急がば回れの精神で。',
                    health: '無理は禁物。休息も仕事のうちと心得て。',
                    lucky: { color: 'ミスティパープル', item: 'ゆっくり煎ったナッツ' }
                },
                {
                    type: '吉',
                    color: 'from-red-400 to-orange-500',
                    overall: 'スパイシーに煎られたピーナッツ!情熱的な一日に。',
                    love: '積極的なアプローチが吉。勇気を出して一歩踏み出して!❤️‍🔥',
                    work: 'リーダーシップを発揮する場面が。自信を持って!',
                    health: 'エネルギッシュに動ける日。アクティブに過ごそう。',
                    lucky: { color: 'ファイアレッド', item: 'スパイシーナッツ' }
                }
            ];

            const crackPeanut = () => {
                setShaking(true);
                
                // 振動フィードバック
                if (navigator.vibrate) {
                    navigator.vibrate([50, 30, 50]);
                }
                
                setTimeout(() => {
                    setShaking(false);
                    setCracked(true);
                    const randomFortune = fortunes[Math.floor(Math.random() * fortunes.length)];
                    setFortune(randomFortune);
                }, 800);
            };

            const reset = () => {
                setCracked(false);
                setFortune(null);
            };

            // 背景画像のパスを設定
            const bgImagePath = './IMG_7110_2.JPG';

            return (
                <div className="min-h-screen relative overflow-hidden" style={{ minHeight: '100vh', minHeight: '100dvh' }}>
                    {/* Background Image with Overlay */}
                    <div 
                        className="absolute inset-0 bg-cover bg-center"
                        style={{
                            backgroundImage: `url('${bgImagePath}')`,
                            filter: 'brightness(0.7)'
                        }}
                    />
                    <div className="absolute inset-0 bg-gradient-to-b from-amber-900/60 via-orange-900/50 to-yellow-900/60" />
                    
                    {/* Content */}
                    <div className="relative z-10 min-h-screen p-8" style={{ minHeight: '100vh', minHeight: '100dvh' }}>
                        <div className="max-w-2xl mx-auto">
                            {/* Header */}
                            <div className="text-center mb-12">
                                <h1 className="text-5xl font-bold text-white mb-2 flex items-center justify-center gap-3 drop-shadow-lg">
                                    🥜ィュ占い🥜
                                </h1>
                                <p className="text-amber-100 text-lg drop-shadow-md">殻を割って、今日の運勢をチェック!</p>
                            </div>

                            {!cracked ? (
                                /* Peanut Animation */
                                <div className="flex flex-col items-center gap-8">
                                    <button
                                        onClick={crackPeanut}
                                        disabled={shaking}
                                        className={`relative transition-all duration-300 hover:scale-110 active:scale-95 ${
                                            shaking ? 'animate-bounce' : ''
                                        }`}
                                    >
                                        <div className="text-9xl filter drop-shadow-2xl cursor-pointer">
                                            🥜
                                        </div>
                                    </button>
                                    
                                    <div className="text-center space-y-4 bg-black/30 backdrop-blur-md rounded-3xl px-8 py-6">
                                        <p className="text-3xl font-semibold text-white drop-shadow-lg">
                                            {shaking ? 'パキッ...!' : 'ピーナッツをタップして割ろう!'}
                                        </p>
                                        {!shaking && (
                                            <p className="text-amber-200 text-lg drop-shadow-md">
                                                ✨ あなたの運勢が待っています ✨
                                            </p>
                                        )}
                                    </div>
                                </div>
                            ) : (
                                /* Fortune Display */
                                <div className="space-y-6 animate-in fade-in duration-700">
                                    {/* Fortune Type Badge */}
                                    <div className="text-center">
                                        <div className={`inline-block px-12 py-6 rounded-3xl bg-gradient-to-r ${fortune.color} text-white shadow-2xl transform hover:scale-105 transition-transform`}>
                                            <div className="text-6xl font-bold mb-2">{fortune.type}</div>
                                            <div className="flex items-center justify-center gap-2 text-xl">
                                                <i data-lucide="sparkles" className="w-6 h-6"></i>
                                                <span>今日の運勢</span>
                                                <i data-lucide="sparkles" className="w-6 h-6"></i>
                                            </div>
                                        </div>
                                    </div>

                                    {/* Overall Fortune */}
                                    <div className="bg-white/95 backdrop-blur-sm rounded-2xl p-6 shadow-2xl border-2 border-amber-200">
                                        <div className="flex items-center gap-3 mb-3">
                                            <i data-lucide="star" className="w-6 h-6 text-amber-500"></i>
                                            <h3 className="text-xl font-bold text-amber-900">総合運</h3>
                                        </div>
                                        <p className="text-gray-700 text-lg leading-relaxed">{fortune.overall}</p>
                                    </div>

                                    {/* Love Fortune */}
                                    <div className="bg-white/95 backdrop-blur-sm rounded-2xl p-6 shadow-2xl border-2 border-pink-200">
                                        <div className="flex items-center gap-3 mb-3">
                                            <i data-lucide="heart" className="w-6 h-6 text-pink-500"></i>
                                            <h3 className="text-xl font-bold text-pink-900">恋愛運</h3>
                                        </div>
                                        <p className="text-gray-700 text-lg leading-relaxed">{fortune.love}</p>
                                    </div>

                                    {/* Work Fortune */}
                                    <div className="bg-white/95 backdrop-blur-sm rounded-2xl p-6 shadow-2xl border-2 border-blue-200">
                                        <div className="flex items-center gap-3 mb-3">
                                            <i data-lucide="briefcase" className="w-6 h-6 text-blue-500"></i>
                                            <h3 className="text-xl font-bold text-blue-900">仕事運</h3>
                                        </div>
                                        <p className="text-gray-700 text-lg leading-relaxed">{fortune.work}</p>
                                    </div>

                                    {/* Health Fortune */}
                                    <div className="bg-white/95 backdrop-blur-sm rounded-2xl p-6 shadow-2xl border-2 border-green-200">
                                        <div className="flex items-center gap-3 mb-3">
                                            <i data-lucide="activity" className="w-6 h-6 text-green-500"></i>
                                            <h3 className="text-xl font-bold text-green-900">健康運</h3>
                                        </div>
                                        <p className="text-gray-700 text-lg leading-relaxed">{fortune.health}</p>
                                    </div>

                                    {/* Lucky Items */}
                                    <div className="bg-gradient-to-r from-amber-100/95 to-yellow-100/95 backdrop-blur-sm rounded-2xl p-6 shadow-2xl border-2 border-amber-300">
                                        <h3 className="text-xl font-bold text-amber-900 mb-4 flex items-center gap-2">
                                            <i data-lucide="sparkles" className="w-6 h-6"></i>
                                            ラッキーアイテム
                                        </h3>
                                        <div className="grid grid-cols-2 gap-4">
                                            <div>
                                                <p className="text-sm text-amber-700 mb-1">ラッキーカラー</p>
                                                <p className="text-lg font-semibold text-amber-900">🎨 {fortune.lucky.color}</p>
                                            </div>
                                            <div>
                                                <p className="text-sm text-amber-700 mb-1">ラッキーアイテム</p>
                                                <p className="text-lg font-semibold text-amber-900">✨ {fortune.lucky.item}</p>
                                            </div>
                                        </div>
                                    </div>

                                    {/* Reset Button */}
                                    <div className="text-center pt-4">
                                        <button
                                            onClick={reset}
                                            className="bg-gradient-to-r from-amber-500 to-orange-500 hover:from-amber-600 hover:to-orange-600 text-white font-bold py-4 px-8 rounded-full shadow-2xl transform hover:scale-105 transition-all text-lg"
                                        >
                                            🥜 もう一度占う
                                        </button>
                                    </div>
                                </div>
                            )}

                            {/* Footer */}
                            <div className="text-center mt-12 bg-black/30 backdrop-blur-md rounded-2xl py-3 px-6 inline-block mx-auto w-full">
                                <p className="text-amber-100 text-sm drop-shadow-md">🥜 毎日新しい運勢をチェックしよう! 🥜</p>
                            </div>
                        </div>
                    </div>
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<PeanutFortune />);
        
        // Lucideアイコンの初期化
        lucide.createIcons();
        
        // Service Worker登録
        if ('serviceWorker' in navigator) {
            window.addEventListener('load', () => {
                navigator.serviceWorker.register('./sw.js')
                    .then(reg => console.log('Service Worker registered'))
                    .catch(err => console.log('Service Worker registration failed'));
            });
        }
    </script>
</body>
</html>
