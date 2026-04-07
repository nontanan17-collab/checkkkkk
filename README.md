<div id="home-page" class="min-h-full p-4 md:p-6 pt-20">
  <div class="max-w-lg mx-auto">
    <div class="flex items-center justify-between mb-8">
      <div>
        <h1 id="shop-title" class="text-2xl md:text-3xl font-bold text-orange-800">🍜 ก๋วยเตี๋ยวเรือรสจนา สาขา 2</h1>
        <p id="txt-daily-check" class="text-orange-600 text-sm mt-1">เช็คสต็อกประจำวัน</p>
      </div>
      <button onclick="showHistory()" class="flex items-center gap-2 bg-white px-4 py-2 rounded-xl shadow-md hover:shadow-lg transition-all text-orange-700 font-medium">
        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
        </svg>
        <span id="txt-history">ประวัติ</span>
      </button>
    </div>

    <div class="bg-white rounded-2xl p-4 shadow-md mb-6">
      <p id="txt-date2" class="text-gray-500 text-sm">วันที่</p>
      <p id="current-date" class="text-lg font-semibold text-gray-800"></p>
    </div>

    <div class="space-y-4">
      <button onclick="selectCategory('ผัก')" class="w-full bg-gradient-to-r from-green-500 to-green-600 text-white p-5 rounded-2xl shadow-lg hover:shadow-xl transition-all transform hover:scale-[1.02] active:scale-[0.98]">
        <div class="flex items-center gap-4">
          <div class="w-14 h-14 bg-white/20 rounded-xl flex items-center justify-center text-3xl">🥬</div>
          <div class="text-left">
            <p id="cat-veg" class="text-xl font-bold">ผัก</p>
            <p id="cat-veg-desc" class="text-green-100 text-sm">เช็คสต็อกผัก</p>
          </div>
          <svg class="w-6 h-6 ml-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
        </div>
      </button>

      <button onclick="selectCategory('น้ำ')" class="w-full bg-gradient-to-r from-cyan-500 to-cyan-600 text-white p-5 rounded-2xl shadow-lg hover:shadow-xl transition-all transform hover:scale-[1.02] active:scale-[0.98]">
        <div class="flex items-center gap-4">
          <div class="w-14 h-14 bg-white/20 rounded-xl flex items-center justify-center text-3xl">🥤</div>
          <div class="text-left">
            <p id="cat-drink" class="text-xl font-bold">น้ำ</p>
            <p id="cat-drink-desc" class="text-cyan-100 text-sm">เช็คสต็อกเครื่องดื่ม</p>
          </div>
          <svg class="w-6 h-6 ml-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
        </div>
      </button>

      <button onclick="selectCategory('เนื้อสัตว์')" class="w-full bg-gradient-to-r from-red-500 to-red-600 text-white p-5 rounded-2xl shadow-lg hover:shadow-xl transition-all transform hover:scale-[1.02] active:scale-[0.98]">
        <div class="flex items-center gap-4">
          <div class="w-14 h-14 bg-white/20 rounded-xl flex items-center justify-center text-3xl">🍖</div>
          <div class="text-left">
            <p id="cat-meat" class="text-xl font-bold">เนื้อสัตว์</p>
            <p id="cat-meat-desc" class="text-red-100 text-sm">เช็คสต็อกเนื้อสัตว์</p>
          </div>
          <svg class="w-6 h-6 ml-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
        </div>
      </button>

      <button onclick="selectCategory('ของสิ้นเปลือง')" class="w-full bg-gradient-to-r from-amber-500 to-amber-600 text-white p-5 rounded-2xl shadow-lg hover:shadow-xl transition-all transform hover:scale-[1.02] active:scale-[0.98]">
        <div class="flex items-center gap-4">
          <div class="w-14 h-14 bg-white/20 rounded-xl flex items-center justify-center text-3xl">🧻</div>
          <div class="text-left">
            <p id="cat-consumable" class="text-xl font-bold">ของสิ้นเปลือง</p>
            <p id="cat-consumable-desc" class="text-amber-100 text-sm">เช็คสต็อกของสิ้นเปลือง</p>
          </div>
          <svg class="w-6 h-6 ml-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
        </div>
      </button>

      <button onclick="selectCategory('ของหวาน')" class="w-full bg-gradient-to-r from-pink-500 to-pink-600 text-white p-5 rounded-2xl shadow-lg hover:shadow-xl transition-all transform hover:scale-[1.02] active:scale-[0.98]">
        <div class="flex items-center gap-4">
          <div class="w-14 h-14 bg-white/20 rounded-xl flex items-center justify-center text-3xl">🍮</div>
          <div class="text-left">
            <p id="cat-dessert" class="text-xl font-bold">ของหวาน</p>
            <p id="cat-dessert-desc" class="text-pink-100 text-sm">เช็คสต็อกของหวาน</p>
          </div>
          <svg class="w-6 h-6 ml-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
          </svg>
        </div>
      </button>
    </div>
  </div>
</div>

<div id="name-page" class="min-h-full p-4 md:p-6 hidden">
  <div class="max-w-lg mx-auto fade-in">
    <button onclick="goHome()" class="flex items-center gap-2 text-orange-700 mb-6 hover:text-orange-800 transition-colors">
      <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
      </svg>
      <span id="txt-back-home">กลับหน้าหลัก</span>
    </button>

    <div class="bg-white rounded-2xl p-6 shadow-lg">
      <div id="category-badge" class="inline-flex items-center gap-2 px-4 py-2 rounded-full text-white text-sm font-medium mb-4"></div>
      <h2 id="txt-staff-name-title" class="text-xl font-bold text-gray-800 mb-2">ผู้เช็คสต็อก</h2>
      <p id="txt-staff-name-desc" class="text-gray-500 mb-6">กรุณากรอกชื่อผู้ทำการเช็คสต็อก</p>
      <div class="space-y-4">
        <div>
          <label id="txt-full-name-label" class="block text-sm font-medium text-gray-700 mb-2">ชื่อ-นามสกุล</label>
          <input type="text" id="checker-name" placeholder="กรอกชื่อของคุณ" class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-orange-500 focus:outline-none transition-colors text-lg">
        </div>
        <button onclick="startChecking()" id="btn-start-checking" class="w-full bg-orange-500 text-white py-4 rounded-xl font-semibold text-lg hover:bg-orange-600 transition-colors shadow-md hover:shadow-lg">เริ่มเช็คสต็อก</button>
      </div>
    </div>
  </div>
</div>

<div id="stock-page" class="min-h-full p-4 md:p-6 hidden">
  <div class="max-w-2xl mx-auto fade-in">
    <div class="flex items-center justify-between mb-6">
      <button onclick="goToNamePage()" class="flex items-center gap-2 text-orange-700 hover:text-orange-800 transition-colors">
        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
        </svg>
        <span id="txt-back">กลับ</span>
      </button>
      <div id="stock-category-badge" class="px-4 py-2 rounded-full text-white text-sm font-medium"></div>
    </div>

    <div class="bg-white rounded-2xl shadow-lg overflow-hidden">
      <div class="bg-gradient-to-r from-orange-500 to-orange-600 p-4 text-white">
        <p class="text-sm opacity-90"><span id="txt-staff-checker">ผู้เช็คสต็อก:</span> <span id="display-checker-name" class="font-semibold"></span></p>
        <p class="text-sm opacity-90"><span id="txt-date-label">วันที่:</span> <span id="display-date" class="font-semibold"></span></p>
      </div>

      <div class="overflow-x-auto">
        <table class="w-full">
          <thead class="bg-gray-50">
            <tr>
              <th id="txt-item" class="px-4 py-3 text-left text-sm font-semibold text-gray-700">รายการ</th>
              <th id="txt-quantity" class="px-4 py-3 text-center text-sm font-semibold text-gray-700 w-28">จำนวน</th>
              <th id="txt-unit" class="px-4 py-3 text-center text-sm font-semibold text-gray-700 w-28">หน่วย</th>
              <th id="txt-note" class="px-4 py-3 text-left text-sm font-semibold text-gray-700">หมายเหตุ</th>
            </tr>
          </thead>
          <tbody id="stock-table-body" class="divide-y divide-gray-100"></tbody>
        </table>
      </div>

      <div class="p-4 bg-gray-50">
        <button id="save-btn" onclick="saveStock()" class="w-full bg-gradient-to-r from-green-500 to-green-600 text-white py-4 rounded-xl font-semibold text-lg hover:from-green-600 hover:to-green-700 transition-all shadow-md hover:shadow-lg flex items-center justify-center gap-2">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
          </svg>
          <span id="txt-save">บันทึกข้อมูล</span>
        </button>
        <p class="text-xs text-gray-500 mt-2">* ช่อง “จำนวน” ใส่ได้เฉพาะ 0-9 และสัญลักษณ์ . / + -</p>
      </div>
    </div>
  </div>
</div>

<div id="history-page" class="min-h-full p-4 md:p-6 hidden">
  <div class="max-w-2xl mx-auto fade-in">
    <button onclick="goHome()" class="flex items-center gap-2 text-orange-700 mb-6 hover:text-orange-800 transition-colors">
      <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
      </svg>
      <span id="txt-back-home2">กลับหน้าหลัก</span>
    </button>

    <h2 id="txt-history-title" class="text-2xl font-bold text-gray-800 mb-4">📋 ประวัติการเช็คสต็อก</h2>

    <div class="bg-white rounded-2xl p-4 shadow-md mb-6">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div>
          <label id="txt-select-date" class="block text-sm font-medium text-gray-700 mb-2">เลือกวันที่</label>
          <input type="date" id="filter-date" onchange="filterHistory()" class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-orange-500 focus:outline-none transition-colors">
        </div>
        <div>
          <label id="txt-category-label" class="block text-sm font-medium text-gray-700 mb-2">หมวดหมู่</label>
          <select id="filter-category" onchange="filterHistory()" class="w-full px-4 py-3 border-2 border-gray-200 rounded-xl focus:border-orange-500 focus:outline-none transition-colors">
            <option value="" id="opt-all">ทั้งหมด</option>
            <option value="ผัก">ผัก</option>
            <option value="น้ำ">น้ำ</option>
            <option value="เนื้อสัตว์">เนื้อสัตว์</option>
            <option value="ของสิ้นเปลือง">ของสิ้นเปลือง</option>
            <option value="ของหวาน">ของหวาน</option>
          </select>
        </div>
      </div>
    </div>

    <div id="history-list" class="space-y-4"></div>
    <div id="no-history" class="hidden text-ce
