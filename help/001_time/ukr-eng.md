<style>
  table {
    border-collapse: collapse;
  }
  
  table.myTable th {
    padding: 5px;
    vertical-align: middle;
  }
  
  table.myTable td {
    border: 1px solid white;
    padding: 5px;
    vertical-align: middle;
  }
  
  .redText {
    color: #C85050;
    font-weight: bold;
  }
  
  .noun {
      color: #AAAAAA;
  }

  .horizontalBlocks {
    display: flex; 
    gap: 10px; 
    align-items: center; 
    padding: 10px;
  }

  .verticalBlocks {
    display: flex;
    flex-direction: column;
    gap: 0px;
  }

  .smallGrayText {
    color: #888888;
    font-size: 10px;
    font-weight: 300;    /* тонкий / light */
  }

  table[data-cell="11"] .c11 { background: rgba(0, 140, 0, 0.3); }
  table[data-cell="12"] .c12 { background: rgba(0, 140, 0, 0.3); }
  table[data-cell="13"] .c13 { background: rgba(0, 140, 0, 0.3); }
  
  table[data-cell="21"] .c21 { background: rgba(0, 140, 0, 0.3); }
  table[data-cell="22"] .c22 { background: rgba(0, 140, 0, 0.3); }
  table[data-cell="23"] .c23 { background: rgba(0, 140, 0, 0.3); }
  
  table[data-cell="31"] .c31 { background: rgba(0, 140, 0, 0.3); }
  table[data-cell="32"] .c32 { background: rgba(0, 140, 0, 0.3); }
  table[data-cell="33"] .c33 { background: rgba(0, 140, 0, 0.3); }

  /* за замовчуванням ховаємо */
  .wrongNounsHelp {
    display: none; 
  }
  
  /* показуємо, якщо таблиця має data-cell="32" */
  .myTable[data-cell="32"] ~ .wrongNounsHelp {
    display: block;
  }

</style>


<table class="myTable" data-cell="32">
    <tr>
        <th>Запитання</th>
        <th>Ствердження</th>
        <th>Заперечення</th>
    </tr>
    <tr>
        <td class="c11">
          <div class="horizontalBlocks">
            <div class="redText">Will</div>
            <div class="noun">I<br>you<br>we<br>they<br>he<br>she</div>
            <div>love?</div>
          </div>
        </td>
        <td class="c12">
          <div class="horizontalBlocks">
            <div class="noun">I<br>you<br>we<br>they<br>he<br>she</div>
            <div class="redText">will</div>
            <div>love</div>
          </div>
        </td>
        <td class="c13">
          <div class="horizontalBlocks">
            <div class="noun">
              I<br>you<br>we<br>they<br>he<br>she
            </div>
            <div class="redText">won't</div>
            <div>love</div>
          </div>
        </td>
        <th class="side-label">
          <div class="verticalBlocks">
            <span>Майбутнє</span>
            <span class ="smallGrayText">won't = will not</span>
          </div>
        </th>
    </tr>
    <tr>
        <td class="c21">
          <div class="verticalBlocks">
            <div class="horizontalBlocks">
              <div class="redText">Do</div>
              <div class="noun">I<br>you<br>we<br>they</div>
              <div>love</div>
            </div>
            <div class="horizontalBlocks">
              <div class="redText">Does</div>
              <div class="noun">he<br>she</div>
              <div>love</div>
            </div>
          </div>
        </td>
        <td class="c22">
          <div class="verticalBlocks">
            <div class="horizontalBlocks">
              <div class="noun">I<br>you<br>we<br>they</div>
              <div>love</div>
            </div>
            <div class="horizontalBlocks">
              <div class="noun">he<br>she</div>
              <div>love<span class="redText">s</span></div>
            </div>
          </div>
        </td>
        <td class="c23">
          <div class="verticalBlocks">
            <div class="horizontalBlocks">
              <div class="noun">I<br>you<br>we<br>they</div>
              <div class="redText">don't</div>
              <div>love</div>
            </div>
            <div class="horizontalBlocks">
              <div class="noun">he<br>she</div>
              <div class="redText">doesn't</div>
              <div>love</div>
            </div>
          </div>
        </td>
        <th class="side-label">
          <div class="verticalBlocks">
            <span>Теперішнє</span>
            <span class ="smallGrayText">don't = do not</span>
            <span class ="smallGrayText">doesn't = does not</span>
          </div>
        </th>
    </tr>
    <tr>
        <td class="c31">
          <div class="horizontalBlocks">
            <div class="redText">Did</div>
            <div class="noun">I<br>you<br>we<br>they<br>he<br>she</div>
            <div>love</div>
          </div>
        </td>
        <td class="c32">
          <div class="horizontalBlocks">
            <div class="noun">I<br>you<br>we<br>they<br>he<br>she</div>
            <div>lov<span class="redText">ed</span></div>
          </div>
        </td>
        <td class="c33">
          <div class="horizontalBlocks">
            <div class="noun">I<br>you<br>we<br>they<br>he<br>she</div>
            <div><span class="redText">didn't</span></div>
            <div>love</div>
          </div>
        </td>
        <th class="side-label">
          <div class="verticalBlocks">
            <span>Минуле</span>
            <span class ="smallGrayText">didn't = did not</span>
          </div>
        </th>
    </tr>
</table>
<br>

<div class="wrongNounsHelp">
  <h2>Правильні та неправильні дієслова</h2>
  <ul>
    <li>Правильні дієслова в минулому часі отримують закінчення <span class="redText">-ed</span>.</li>
    <li>Неправильні дієслова можуть виглядати будь-як і їх варто запам'ятати</li>
  </ul>
</div>

