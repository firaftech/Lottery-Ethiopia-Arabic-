<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Claim Your 1 Million Birr Prize!</title>
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-gradient-to-br from-slate-950 via-indigo-950 to-neutral-950 min-h-screen flex items-center justify-center p-4 pt-16 pb-8 font-sans">

    <!-- MAIN REGISTRATION CARD -->
    <div id="form-card" class="w-full max-w-md bg-slate-900/80 backdrop-blur-md border border-slate-800 rounded-2xl p-8 pt-14 shadow-2xl relative overflow-visible transition-all duration-300">
        
        <!-- OWNER PROFILE IMAGE (From 29914.jpg) WITH ETHIOPIAN FLAG -->
        <div class="absolute -top-16 left-1/2 transform -translate-x-1/2 z-20">
            <div class="w-28 h-28 rounded-full p-1 bg-gradient-to-tr from-emerald-400 via-amber-400 to-red-500 shadow-xl shadow-slate-950/50 relative">
                <img 
                    src="29914.jpg" 
                    alt="Official Owner" 
                    class="w-full h-full object-cover rounded-full border-4 border-slate-900"
                />
                
                <!-- Circular Ethiopian Flag Badge -->
                <div class="absolute -top-1 -right-1 w-8 h-8 rounded-full border-2 border-slate-900 shadow-md flex flex-col overflow-hidden">
                    <div class="h-1/3 bg-[#009a44]"></div>
                    <div class="h-1/3 bg-[#fed100]"></div>
                    <div class="h-1/3 bg-[#ef4444]"></div>
                </div>
            </div>
            
            <!-- Verification Badge Icon -->
            <span class="absolute bottom-1 right-1 bg-emerald-500 text-slate-950 text-xs w-6 h-6 rounded-full flex items-center justify-center border-2 border-slate-900 shadow font-bold">
                <i class="fa-solid fa-check"></i>
            </span>
        </div>

        <!-- Decorative Top Glow -->
        <div class="absolute -top-10 -left-10 w-40 h-40 bg-emerald-500/10 rounded-full blur-3xl"></div>
        <div class="absolute -top-10 -right-10 w-40 h-40 bg-amber-500/10 rounded-full blur-3xl"></div>

        <!-- Header -->
        <div class="text-center mb-8 relative z-10 mt-2">
            <h1 class="text-lg font-bold text-white tracking-wide">Mohammed Al-Qahtani</h1>
            <p class="text-xs font-semibold text-amber-400 uppercase tracking-widest mb-4 opacity-80">Owner / Admin</p>
            
            <div class="inline-flex items-center justify-center w-12 h-12 bg-slate-800/80 border border-slate-700/50 rounded-full mb-3 text-amber-400">
                <i class="fa-solid fa-trophy text-xl"></i>
            </div>
            
            <h2 class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-emerald-400 via-amber-300 to-red-400 tracking-tight">
                1 Million Birr Giveaway!
            </h2>
            <p class="text-slate-300 mt-2 text-sm font-medium px-4">
                Exclusive reward for 1 million Ethiopian residents living in Arabia.
            </p>
        </div>

        <!-- Form -->
        <form class="space-y-6 relative z-10" onsubmit="handleSubmit(event)">
            
            <!-- Full Name Input -->
            <div>
                <label for="full-name" class="block text-xs font-semibold uppercase tracking-wider text-slate-300 mb-2">
                    Full Name <span class="text-amber-400">*</span>
                </label>
                <div class="relative">
                    <span class="absolute inset-y-0 left-0 flex items-center pl-4 text-slate-500">
                        <i class="fa-solid fa-user"></i>
                    </span>
                    <input 
                        type="text" 
                        id="full-name" 
                        required
                        placeholder="e.g., Abebe Bikila" 
                        class="w-full pl-11 pr-4 py-3 bg-slate-800/60 border border-slate-700 rounded-xl text-white placeholder-slate-500 focus:outline-none focus:ring-2 focus:ring-amber-400 focus:border-transparent transition-all duration-200"
                    />
                </div>
                <p class="text-xs text-slate-500 mt-1">Must exactly match your legal bank account name.</p>
            </div>

            <!-- Country Selection Dropdown -->
            <div>
                <label for="country" class="block text-xs font-semibold uppercase tracking-wider text-slate-300 mb-2">
                    Current Country in Arabia <span class="text-amber-400">*</span>
                </label>
                <div class="relative">
                    <span class="absolute inset-y-0 left-0 flex items-center pl-4 text-slate-500">
                        <i class="fa-solid fa-earth-meast"></i>
                    </span>
                    <select 
                        id="country" 
                        required
                        class="w-full pl-11 pr-10 py-3 bg-slate-800/60 border border-slate-700 rounded-xl text-white focus:outline-none focus:ring-2 focus:ring-amber-400 focus:border-transparent transition-all duration-200 appearance-none cursor-pointer"
                    >
                        <option value="" disabled selected class="text-slate-500 bg-slate-900">Choose your country</option>
                        <option value="ae" class="bg-slate-900">United Arab Emirates</option>
                        <option value="sa" class="bg-slate-900">Saudi Arabia</option>
                        <option value="qa" class="bg-slate-900">Qatar</option>
                        <option value="jo" class="bg-slate-900">Jordan</option>
                        <option value="bh" class="bg-slate-900">Bahrain</option>
                        <option value="tr" class="bg-slate-900">Turkey</option>
                        <option value="om" class="bg-slate-900">Oman</option>
                    </select>
                    <span class="absolute inset-y-0 right-0 flex items-center pr-4 text-slate-400 pointer-events-none">
                        <i class="fa-solid fa-chevron-down text-xs"></i>
                    </span>
                </div>
            </div>

            <!-- Bank Account Number Input -->
            <div>
                <label for="account-number" class="block text-xs font-semibold uppercase tracking-wider text-slate-300 mb-2">
                    Bank Account Number / IBAN <span class="text-amber-400">*</span>
                </label>
                <div class="relative">
                    <span class="absolute inset-y-0 left-0 flex items-center pl-4 text-slate-500">
                        <i class="fa-solid fa-building-columns"></i>
                    </span>
                    <input 
                        type="text" 
                        id="account-number" 
                        required
                        placeholder="Enter account number or IBAN" 
                        class="w-full pl-11 pr-4 py-3 bg-slate-800/60 border border-slate-700 rounded-xl text-white placeholder-slate-500 focus:outline-none focus:ring-2 focus:ring-amber-400 focus:border-transparent transition-all duration-200 tracking-wider font-mono text-sm"
                    />
                </div>
            </div>

            <!-- Trust Badge -->
            <div class="bg-slate-800/40 border border-slate-700/50 rounded-xl p-3 flex items-start space-x-3">
                <i class="fa-solid fa-shield-halved text-amber-400 mt-0.5 text-sm"></i>
                <p class="text-xs text-slate-400 leading-relaxed">
                    Your data is protected with 256-bit bank-grade encryption. We will never share your personal account details.
                </p>
            </div>

            <!-- Submit Button -->
            <button 
                type="submit" 
                class="w-full py-3.5 px-4 bg-gradient-to-r from-emerald-500 via-amber-400 to-red-500 hover:opacity-90 text-slate-950 font-extrabold rounded-xl shadow-lg transform hover:-translate-y-0.5 active:translate-y-0 transition-all duration-150 tracking-wide text-sm cursor-pointer"
            >
                CLAIM MY 1,000,000 BIRR NOW
            </button>
        </form>
    </div>


    <!-- CUSTOM SUCCESS MODAL WITH UNIQUE LOTTERY NUMBER -->
    <div id="success-modal" class="hidden fixed inset-0 bg-slate-950/80 backdrop-blur-sm flex items-center justify-center p-4 z-50">
        <div class="w-full max-w-sm bg-slate-900 border border-amber-500/30 rounded-2xl p-6 text-center shadow-2xl relative overflow-hidden transform scale-95 transition-all duration-300">
            
            <!-- Success Animation Ring -->
            <div class="inline-flex items-center justify-center w-16 h-16 bg-emerald-500/10 border border-emerald-500/30 rounded-full mb-3">
                <i class="fa-solid fa-ticket text-2xl text-emerald-400"></i>
            </div>

            <!-- Message Details -->
            <h3 class="text-xl font-bold text-white mb-1">Registration Confirmed!</h3>
            <p class="text-xs text-slate-400 mb-4">Your unique lottery reference has been generated:</p>

            <!-- Unique Generated Lottery Number Field -->
            <div class="bg-slate-950 border border-slate-800 rounded-xl py-3 px-4 mb-4 shadow-inner">
                <span class="text-slate-500 font-mono text-xs block tracking-widest uppercase mb-1">Your Unique Lottery ID</span>
                <span id="lottery-number" class="text-2xl font-black font-mono tracking-widest text-amber-300">#ET-000000</span>
            </div>

            <p class="text-xs text-slate-300 leading-relaxed px-2">
                The grand prize of <span class="text-amber-400 font-bold">1 Million Birr</span> will be sent directly to your registered bank account <span class="text-emerald-400 font-bold">after 1 day</span> once verification matches this unique ticket.
            </p>

            <!-- Separation Line -->
            <div class="border-t border-slate-800 my-4"></div>

            <!-- Close Button -->
            <button 
                onclick="closeModal()" 
                class="w-full py-2.5 px-4 bg-slate-800 hover:bg-slate-700 text-white font-medium rounded-xl transition-all duration-150 text-sm cursor-pointer"
            >
                Done
            </button>
        </div>
    </div>


    <!-- JAVASCRIPT FOR GENERATING RANDOM LOTTERY ID & SHOW MODAL -->
    <script>
        function generateLotteryNumber() {
            // Generates a random 6-digit number between 100000 and 999999
            const randomNumber = Math.floor(100000 + Math.random() * 900000);
            return `#ET-${randomNumber}`;
        }

        function handleSubmit(event) {
            event.preventDefault(); 
            
            // Set the unique number in the modal
            document.getElementById('lottery-number').innerText = generateLotteryNumber();

            // Open the custom success modal
            const modal = document.getElementById('success-modal');
            modal.classList.remove('hidden');
            setTimeout(() => {
                modal.firstElementChild.classList.remove('scale-95');
                modal.firstElementChild.classList.add('scale-100');
            }, 10);
        }

        function closeModal() {
            const modal = document.getElementById('success-modal');
            modal.firstElementChild.classList.remove('scale-100');
            modal.firstElementChild.classList.add('scale-95');
            setTimeout(() => {
                modal.classList.add('hidden');
            }, 150);
        }
    </script>

</body>
</html>

