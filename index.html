<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kalkulator PPh by Adien</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --gemini-bg: #131314;
            --gemini-card: #1e1f20;
            --gemini-blue: #4e95ff;
            --gemini-purple: #9d7aff;
            --gemini-text: #e3e3e3;
            --gemini-text-dim: #b4b4b4;
            --island-bg: #2f2f30;
            --input-bg: #131314;
            --border-color: #333333;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--gemini-bg);
            color: var(--gemini-text);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        /* --- README & INFO OVERLAY --- */
        .overlay {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0, 0, 0, 0.85);
            backdrop-filter: blur(10px);
            z-index: 9999;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 1;
            transition: opacity 0.3s ease;
        }

        .modal-content {
            background: var(--gemini-card);
            padding: 32px;
            border-radius: 28px;
            max-width: 450px;
            width: 90%;
            border: 1px solid var(--border-color);
            box-shadow: 0 20px 50px rgba(0,0,0,0.5);
        }

        .modal-content h2 { 
            font-size: 20px; margin-bottom: 12px;
            background: linear-gradient(90deg, var(--gemini-blue), var(--gemini-purple));
            -webkit-background-clip: text; -webkit-text-fill-color: transparent;
        }

        .modal-content p, .modal-content li { color: var(--gemini-text-dim); font-size: 14px; line-height: 1.6; }
        .modal-content ul { margin: 15px 0; padding-left: 20px; }
        .modal-content li { margin-bottom: 8px; }

        .btn-action {
            width: 100%; padding: 14px; background: white; color: black;
            border: none; border-radius: 100px; font-weight: 600; cursor: pointer;
            margin-top: 20px; transition: 0.2s;
        }

        /* --- MAIN CONTAINER --- */
        .container {
            background: var(--gemini-card);
            padding: 40px;
            border-radius: 28px;
            width: 100%;
            max-width: 460px;
            border: 1px solid var(--border-color);
            position: relative;
        }

        .dynamic-island {
            width: 130px; height: 32px; background: var(--island-bg);
            border-radius: 100px; margin: -20px auto 30px;
            display: flex; align-items: center; justify-content: center;
            color: white; font-size: 11px; font-weight: 500;
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .island-active { width: 260px; height: 40px; background: linear-gradient(90deg, #1a73e8, #7b1fa2); }

        h1 { text-align: center; font-size: 22px; font-weight: 600; margin-bottom: 30px; }

        .input-box { margin-bottom: 20px; }
        
        .label-wrapper { display: flex; align-items: center; margin-bottom: 8px; padding-left: 4px; }
        label { font-size: 13px; color: var(--gemini-text-dim); }
        
        .info-icon {
            display: inline-flex;
            align-items: center; justify-content: center;
            width: 16px; height: 16px;
            background: #444; color: #fff;
            border-radius: 50%; font-size: 11px;
            margin-left: 8px; cursor: pointer;
            transition: 0.2s;
        }
        .info-icon:hover { background: var(--gemini-blue); }

        input {
            width: 100%; padding: 16px; border: 1.5px solid #444; border-radius: 16px;
            font-size: 16px; background: var(--input-bg); color: white; transition: 0.3s;
        }
        input:focus { outline: none; border-color: var(--gemini-blue); }

        .btn-calc { 
            width: 100%; padding: 16px; 
            background: linear-gradient(135deg, var(--gemini-blue), var(--gemini-purple)); 
            color: white; border: none; border-radius: 100px; 
            font-size: 16px; font-weight: 600; cursor: pointer; margin-top: 10px;
        }

        /* --- RESULTS --- */
        .result-area { margin-top: 30px; display: none; animation: fadeIn 0.4s ease; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        .res-card { background: rgba(255,255,255,0.03); padding: 25px; border-radius: 20px; text-align: center; border: 1px solid var(--border-color); }
        .res-total-val { font-size: 34px; font-weight: 700; margin: 8px 0; }
        .monthly-label { font-size: 14px; color: var(--gemini-blue); font-weight: 500; }

        .tier-item { display: flex; justify-content: space-between; padding: 10px 0; font-size: 13px; border-bottom: 1px solid rgba(255,255,255,0.05); }
        .tier-item:last-child { border-bottom: none; }
    </style>
</head>
<body>

    <div id="readmeOverlay" class="overlay">
        <div class="modal-content">
            <h2>Kalkulator PPh by Adien</h2>
            <p>Hitung estimasi pajak penghasilan Anda dengan rincian transparan sesuai UU HPP terbaru. Masukkan data tahunan Anda untuk memulai.</p>
            <button class="btn-action" onclick="closeModal('readmeOverlay')">Mulai Menghitung</button>
        </div>
    </div>

    <div id="infoOverlay" class="overlay" style="display: none; opacity: 0;">
        <div class="modal-content">
            <h2>Tentang Tanggungan</h2>
            <p>Tanggungan adalah anggota keluarga sedarah atau semenda yang tidak memiliki penghasilan dan sepenuhnya menjadi tanggungan Anda. Maksimal adalah 3 orang.</p>
            <ul>
                <li><b>Istri:</b> Jika istri tidak bekerja/tidak menggabung NPWP.</li>
                <li><b>Anak:</b> Anak kandung atau anak angkat (belum bekerja).</li>
                <li><b>Orang Tua:</b> Ayah/ibu kandung atau mertua yang sudah tidak berpenghasilan.</li>
            </ul>
            <button class="btn-action" onclick="closeModal('infoOverlay')">Mengerti</button>
        </div>
    </div>

    <div class="container">
        <div class="dynamic-island" id="island">ADIEN TAX PRO</div>
        <h1>Kalkulator PPh 21</h1>

        <div class="input-box">
            <div class="label-wrapper">
                <label>Penghasilan Bruto (Setahun)</label>
            </div>
            <input type="text" id="gajiDisplay" placeholder="Rp 0" oninput="formatInputRupiah(this)">
            <input type="hidden" id="gaji">
        </div>

        <div class="input-box">
            <div class="label-wrapper">
                <label>Jumlah Tanggungan</label>
                <div class="info-icon" onclick="openModal('infoOverlay')">?</div>
            </div>
            <input type="number" id="tanggungan" min="0" max="3" value="0">
        </div>

        <button class="btn-calc" onclick="hitungPajak()">Hitung & Lihat Rincian</button>

        <div id="hasil" class="result-area">
            <div class="res-card">
                <span style="font-size: 12px; color: var(--gemini-text-dim);">PAJAK TAHUNAN</span>
                <div class="res-total-val" id="resPajakTahun"></div>
                <div class="monthly-label">± <span id="resPajakBulan"></span> / Bulan</div>
            </div>

            <div style="margin-top: 20px; padding: 10px;">
                <div id="tierDetails"></div>
                <div class="tier-item" style="border-top: 1px solid var(--border-color); margin-top: 10px; padding-top: 15px;">
                    <span style="font-weight: 600;">PKP:</span>
                    <span id="resPkp" style="color: var(--gemini-purple); font-weight: 700;"></span>
                </div>
            </div>
        </div>
    </div>

    <script>
        function openModal(id) {
            const el = document.getElementById(id);
            el.style.display = 'flex';
            setTimeout(() => el.style.opacity = '1', 10);
        }

        function closeModal(id) {
            const el = document.getElementById(id);
            el.style.opacity = '0';
            setTimeout(() => el.style.display = 'none', 300);
        }

        document.addEventListener('keypress', (e) => {
            if (e.key === 'Enter') hitungPajak();
        });

        function formatInputRupiah(input) {
            let value = input.value.replace(/[^,\d]/g, '');
            document.getElementById('gaji').value = value;
            if (value) {
                input.value = new Intl.NumberFormat('id-ID', {
                    style: 'currency', currency: 'IDR', minimumFractionDigits: 0
                }).format(parseInt(value));
            }
        }

        function hitungPajak() {
            const gaji = parseFloat(document.getElementById('gaji').value) || 0;
            const tanggungan = Math.min(parseInt(document.getElementById('tanggungan').value) || 0, 3);
            const island = document.getElementById('island');

            if (gaji <= 0) {
                island.innerText = "INPUT DATA DULU";
                island.style.background = "#ea4335";
                setTimeout(() => { island.innerText = "ADIEN TAX PRO"; island.style.background = "#2f2f30"; }, 2000);
                return;
            }

            island.classList.add('island-active');
            island.innerText = "ANALYZING...";

            setTimeout(() => {
                const ptkp = 54000000 + (tanggungan * 4500000);
                const pkp = Math.max(0, gaji - ptkp);

                const L1 = 60000000, L2 = 190000000, L3 = 250000000, L4 = 500000000, L5 = 5000000000;
                const p1 = Math.min(pkp, L1) * 0.05;
                const p2 = Math.max(Math.min(pkp - L1, L2), 0) * 0.15;
                const p3 = Math.max(Math.min(pkp - (L1 + L2), L3), 0) * 0.25;
                const p4 = Math.max(Math.min(pkp - L4, L4), 0) * 0.30;
                const p5 = Math.max(pkp - L5, 0) * 0.35;

                const total = p1 + p2 + p3 + p4 + p5;
                const fmt = (n) => new Intl.NumberFormat('id-ID', { style: 'currency', currency: 'IDR', minimumFractionDigits: 0 }).format(n);

                let detailHtml = "";
                [p1, p2, p3, p4, p5].forEach((p, i) => {
                    if (p > 0) detailHtml += `<div class="tier-item"><span style="color: var(--gemini-text-dim)">Lapisan ${i+1}</span><span style="font-weight: 600;">${fmt(p)}</span></div>`;
                });

                document.getElementById('hasil').style.display = 'block';
                document.getElementById('tierDetails').innerHTML = detailHtml || "Nihil";
                document.getElementById('resPkp').innerText = fmt(pkp);
                document.getElementById('resPajakTahun').innerText = fmt(total);
                document.getElementById('resPajakBulan').innerText = fmt(total/12);

                island.innerText = "DONE ✨";
                setTimeout(() => { island.classList.remove('island-active'); island.innerText = "ADIEN TAX PRO"; }, 1500);
            }, 600);
        }
    </script>
</body>
</html>
