<!DOCTYPE html>
<html lang="zh-CN">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>加密货币固定风险交易计算器</title>
    <style>
      :root {
        --primary-color: #2563eb;
        --secondary-color: #eef2ff;
        --border-color: #e2e8f0;
        --warning-color: #ef4444;
        --success-color: #10b981;
        --text-color: #1e293b;
        --background-color: #f8fafc;
      }

      body {
        font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
        line-height: 1.6;
        color: var(--text-color);
        background-color: var(--background-color);
        margin: 0;
        padding: 0;
      }

      .container {
        max-width: 1000px;
        margin: 0 auto;
        padding: 20px;
      }

      header {
        text-align: center;
        margin-bottom: 30px;
        padding-bottom: 20px;
        border-bottom: 1px solid var(--border-color);
      }

      h1 {
        color: var(--primary-color);
        margin-bottom: 10px;
      }

      .description {
        color: #64748b;
        max-width: 800px;
        margin: 0 auto;
      }

      .form-container {
        background-color: white;
        border-radius: 8px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        padding: 25px;
        margin-bottom: 30px;
      }

      .form-row {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 20px;
        margin-bottom: 20px;
      }

      .form-group {
        margin-bottom: 15px;
      }

      label {
        display: block;
        margin-bottom: 5px;
        font-weight: 600;
      }

      input,
      select {
        width: 100%;
        padding: 10px;
        border: 1px solid var(--border-color);
        border-radius: 4px;
        font-size: 16px;
      }

      input:focus {
        outline: none;
        border-color: var(--primary-color);
        box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
      }

      .submit-row {
        text-align: center;
        margin-top: 25px;
      }

      button {
        background-color: var(--primary-color);
        color: white;
        border: none;
        padding: 12px 24px;
        font-size: 16px;
        font-weight: 600;
        border-radius: 4px;
        cursor: pointer;
        transition: background-color 0.2s;
      }

      button:hover {
        background-color: #1d4ed8;
      }

      .results-container {
        display: none;
        background-color: white;
        border-radius: 8px;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        padding: 25px;
        margin-top: 30px;
      }

      .results-header {
        text-align: center;
        margin-bottom: 25px;
      }

      .results-grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 30px;
      }

      .result-section {
        margin-bottom: 25px;
      }

      .result-section h3 {
        color: var(--primary-color);
        border-bottom: 1px solid var(--border-color);
        padding-bottom: 8px;
        margin-bottom: 15px;
      }

      .result-row {
        display: flex;
        justify-content: space-between;
        margin-bottom: 10px;
      }

      .result-label {
        font-weight: 600;
      }

      .trade-summary {
        background-color: var(--secondary-color);
        border-radius: 8px;
        padding: 20px;
        margin: 30px 0;
      }

      .trade-summary h3 {
        color: var(--primary-color);
        margin-top: 0;
        margin-bottom: 15px;
        text-align: center;
      }

      .summary-item {
        display: flex;
        justify-content: space-between;
        padding: 10px 0;
        border-bottom: 1px solid #ddd;
      }

      .summary-item:last-child {
        border-bottom: none;
      }

      .summary-label {
        font-weight: 600;
      }

      .summary-value {
        font-weight: 700;
      }

      .highlight {
        font-size: 1.2em;
        color: var(--primary-color);
      }

      .warning-message {
        color: var(--warning-color);
        padding: 12px;
        background-color: #fef2f2;
        border-radius: 4px;
        margin-top: 15px;
        font-weight: 600;
      }

      .success-message {
        color: var(--success-color);
        padding: 12px;
        background-color: #ecfdf5;
        border-radius: 4px;
        margin-top: 15px;
        font-weight: 600;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <header>
        <h1>加密货币固定风险交易计算器</h1>
        <p class="description">
          基于账户百分比风险管理的交易策略计算工具，确保每笔交易的最大损失不超过账户总额的设定百分比。
        </p>
      </header>

      <div class="form-container">
        <form id="tradingForm">
          <div class="form-row">
            <div class="form-group">
              <label for="assetSymbol">币种符号</label>
              <input type="text" id="assetSymbol" placeholder="例如: BTC, ETH, SOL" value="BTC" required />
            </div>
            <div class="form-group">
              <label for="minOrderSize">最小下单单位</label>
              <input
                type="number"
                id="minOrderSize"
                placeholder="例如: BTC为0.001，ETH为0.01"
                value="0.001"
                step="0.0001"
                min="0.0001"
                required
              />
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label for="currentPrice">当前价格 (USD)</label>
              <input type="number" id="currentPrice" placeholder="输入当前市场价格" step="0.01" min="0.01" required />
            </div>
            <div class="form-group">
              <label for="targetPrice">目标价格 (USD)</label>
              <input type="number" id="targetPrice" placeholder="输入预期目标价格" step="0.01" min="0.01" required />
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label for="stopLossPrice">止损价格 (USD)</label>
              <input type="number" id="stopLossPrice" placeholder="输入止损价格" step="0.01" min="0.01" required />
            </div>
            <div class="form-group">
              <label for="accountBalance">账户总余额 (USD)</label>
              <input type="number" id="accountBalance" placeholder="输入账户总余额" step="0.01" min="1" required />
            </div>
          </div>

          <div class="form-row">
            <div class="form-group">
              <label for="maxBalanceRiskPercent">最大风险百分比 (%)</label>
              <input
                type="number"
                id="maxBalanceRiskPercent"
                placeholder="账户总额的风险百分比"
                value="2"
                step="0.1"
                min="0.1"
                max="100"
                required
              />
            </div>
            <div class="form-group">
              <label for="availableLeverage">杠杆倍数</label>
              <input
                type="number"
                id="availableLeverage"
                placeholder="可用杠杆倍数"
                value="10"
                step="1"
                min="1"
                required
              />
            </div>
          </div>

          <div class="submit-row">
            <button type="submit">计算交易策略</button>
          </div>
        </form>
      </div>

      <div id="results" class="results-container">
        <div class="results-header">
          <h2>交易策略结果</h2>
        </div>

        <div class="trade-summary">
          <h3>📌 交易概要</h3>
          <div class="summary-item">
            <span class="summary-label">交易方向:</span>
            <span id="tradeDirection" class="summary-value highlight"></span>
          </div>
          <div class="summary-item">
            <span class="summary-label">建议交易数量:</span>
            <span id="assetQuantity" class="summary-value highlight"></span>
          </div>
          <div class="summary-item">
            <span class="summary-label">杠杆倍数:</span>
            <span id="summaryLeverage" class="summary-value"></span>
          </div>
          <div class="summary-item">
            <span class="summary-label">最大亏损:</span>
            <span id="maxLossInfo" class="summary-value"></span>
          </div>
          <div class="summary-item">
            <span class="summary-label">盈亏比:</span>
            <span id="riskRewardRatio" class="summary-value"></span>
          </div>
        </div>

        <div id="warningMessages">
          <!-- 警告信息将在这里动态添加 -->
        </div>

        <div class="results-grid">
          <div class="result-section">
            <h3>💰 账户与风险信息</h3>
            <div class="result-row">
              <span class="result-label">账户余额:</span>
              <span id="resultAccountBalance"></span>
            </div>
            <div class="result-row">
              <span class="result-label">最大允许亏损:</span>
              <span id="maxAllowedLoss"></span>
            </div>
            <div class="result-row">
              <span class="result-label">实际最大亏损:</span>
              <span id="actualMaxLoss"></span>
            </div>
            <div class="result-row">
              <span class="result-label">可用杠杆:</span>
              <span id="resultLeverage"></span>
            </div>
          </div>

          <div class="result-section">
            <h3>📊 价格信息</h3>
            <div class="result-row">
              <span class="result-label">当前价格:</span>
              <span id="resultCurrentPrice"></span>
            </div>
            <div class="result-row">
              <span class="result-label">目标价格:</span>
              <span id="resultTargetPrice"></span>
            </div>
            <div class="result-row">
              <span class="result-label">止损价格:</span>
              <span id="resultStopLossPrice"></span>
            </div>
          </div>

          <div class="result-section">
            <h3>🔄 交易策略</h3>
            <div class="result-row">
              <span class="result-label">交易方向:</span>
              <span id="resultTradeDirection"></span>
            </div>
            <div class="result-row">
              <span class="result-label">建议交易数量:</span>
              <span id="resultAssetQuantity"></span>
            </div>
            <div class="result-row">
              <span class="result-label">名义头寸价值:</span>
              <span id="notionalValue"></span>
            </div>
            <div class="result-row">
              <span class="result-label">所需保证金:</span>
              <span id="marginRequired"></span>
            </div>
          </div>

          <div class="result-section">
            <h3>⚖️ 风险收益分析</h3>
            <div class="result-row">
              <span class="result-label">最大收益:</span>
              <span id="maxProfit"></span>
            </div>
            <div class="result-row">
              <span class="result-label">最大损失:</span>
              <span id="maxLoss"></span>
            </div>
            <div class="result-row">
              <span class="result-label">盈亏比:</span>
              <span id="resultRiskRewardRatio"></span>
            </div>
          </div>
        </div>
      </div>
    </div>

    <script>
      /**
       * 计算固定风险的加密货币永续合约杠杆交易策略
       */
      function calculateFixedRiskTrade(
        currentPrice,
        targetPrice,
        stopLossPrice,
        accountBalance,
        maxBalanceRiskPercent = 2,
        availableLeverage,
        minOrderSize = 0.001
      ) {
        // 计算固定风险金额（账户总余额 * 风险百分比）
        const fixedRiskAmount = accountBalance * (maxBalanceRiskPercent / 100);

        // 确定交易方向
        const isLong = targetPrice > currentPrice;
        const tradeDirection = isLong ? "做多 (Long)" : "做空 (Short)";

        // 计算止损距离的百分比（用于显示）
        let stopLossPercentage;
        if (isLong) {
          // 做多时，止损价格应低于当前价格
          if (stopLossPrice >= currentPrice) {
            throw new Error("做多交易的止损价格必须低于当前价格");
          }
          stopLossPercentage = (currentPrice - stopLossPrice) / currentPrice;
        } else {
          // 做空时，止损价格应高于当前价格
          if (stopLossPrice <= currentPrice) {
            throw new Error("做空交易的止损价格必须高于当前价格");
          }
          stopLossPercentage = (stopLossPrice - currentPrice) / currentPrice;
        }

        // 计算每个币的价格变动幅度(绝对值)
        const priceChangePerCoin = Math.abs(currentPrice - stopLossPrice);

        // 计算在不考虑杠杆的情况下，可以承担风险的资产数量
        // 固定风险金额 / 每个币的价格变动 = 可以购买的币数
        const rawAssetQuantity = fixedRiskAmount / priceChangePerCoin;

        // 根据最小下单单位向下取整
        const assetQuantityRounded = Math.floor(rawAssetQuantity / minOrderSize) * minOrderSize;

        // 计算实际的名义头寸价值
        const actualNotionalValue = assetQuantityRounded * currentPrice;

        // 计算实际需要的保证金（名义价值 / 杠杆）
        const actualMarginRequired = actualNotionalValue / availableLeverage;

        // 检查保证金是否超过账户余额
        const isSufficientBalance = actualMarginRequired <= accountBalance;

        // 计算盈利目标的百分比
        let targetProfitPercentage;
        if (isLong) {
          targetProfitPercentage = (targetPrice - currentPrice) / currentPrice;
        } else {
          targetProfitPercentage = (currentPrice - targetPrice) / currentPrice;
        }

        // 计算最大收益
        const maxProfit = assetQuantityRounded * Math.abs(targetPrice - currentPrice);

        // 计算实际的最大损失（应该接近固定风险金额）
        const actualMaxLoss = assetQuantityRounded * priceChangePerCoin;

        // 计算实际的余额风险百分比
        const actualBalanceRiskPercent = (actualMaxLoss / accountBalance) * 100;

        // 计算盈亏比
        const riskRewardRatio = maxProfit / actualMaxLoss;
        const isRecommended = riskRewardRatio >= 1.5;

        // 返回计算结果
        return {
          tradeDirection,
          assetQuantity: assetQuantityRounded,
          notionalPositionValue: actualNotionalValue,
          marginRequired: actualMarginRequired,
          availableLeverage,
          maxProfit,
          maxLoss: actualMaxLoss,
          riskRewardRatio,
          isRecommended,
          isSufficientBalance,
          stopLossPercentage,
          targetProfitPercentage,
          fixedRiskAmount,
          maxBalanceRiskPercent,
          actualBalanceRiskPercent,
        };
      }

      // 格式化显示金额
      function formatCurrency(amount) {
        return new Intl.NumberFormat("en-US", {
          style: "currency",
          currency: "USD",
          minimumFractionDigits: 2,
          maximumFractionDigits: 2,
        }).format(amount);
      }

      // 格式化百分比
      function formatPercent(value) {
        return new Intl.NumberFormat("en-US", {
          style: "percent",
          minimumFractionDigits: 2,
          maximumFractionDigits: 2,
        }).format(value / 100);
      }

      // 处理表单提交
      document.getElementById("tradingForm").addEventListener("submit", function (e) {
        e.preventDefault();

        try {
          const assetSymbol = document.getElementById("assetSymbol").value;
          const currentPrice = parseFloat(document.getElementById("currentPrice").value);
          const targetPrice = parseFloat(document.getElementById("targetPrice").value);
          const stopLossPrice = parseFloat(document.getElementById("stopLossPrice").value);
          const accountBalance = parseFloat(document.getElementById("accountBalance").value);
          const maxBalanceRiskPercent = parseFloat(document.getElementById("maxBalanceRiskPercent").value);
          const availableLeverage = parseInt(document.getElementById("availableLeverage").value);
          const minOrderSize = parseFloat(document.getElementById("minOrderSize").value);

          const result = calculateFixedRiskTrade(
            currentPrice,
            targetPrice,
            stopLossPrice,
            accountBalance,
            maxBalanceRiskPercent,
            availableLeverage,
            minOrderSize
          );

          // 显示结果容器
          document.getElementById("results").style.display = "block";

          // 填充交易概要
          document.getElementById("tradeDirection").textContent = result.tradeDirection;
          document.getElementById("assetQuantity").textContent = `${result.assetQuantity} ${assetSymbol}`;
          document.getElementById("summaryLeverage").textContent = `${result.availableLeverage}x`;
          document.getElementById("maxLossInfo").textContent = `账户的 ${result.actualBalanceRiskPercent.toFixed(
            2
          )}% (${formatCurrency(result.maxLoss)})`;
          document.getElementById("riskRewardRatio").textContent = result.riskRewardRatio.toFixed(2);

          // 填充详细结果
          document.getElementById("resultAccountBalance").textContent = formatCurrency(accountBalance);
          document.getElementById(
            "maxAllowedLoss"
          ).textContent = `账户总余额的 ${maxBalanceRiskPercent}% (${formatCurrency(result.fixedRiskAmount)})`;
          document.getElementById(
            "actualMaxLoss"
          ).textContent = `账户总余额的 ${result.actualBalanceRiskPercent.toFixed(2)}% (${formatCurrency(
            result.maxLoss
          )})`;
          document.getElementById("resultLeverage").textContent = `${result.availableLeverage}x`;

          document.getElementById("resultCurrentPrice").textContent = formatCurrency(currentPrice);
          document.getElementById("resultTargetPrice").textContent = `${formatCurrency(targetPrice)} (${(
            result.targetProfitPercentage * 100
          ).toFixed(2)}%)`;
          document.getElementById("resultStopLossPrice").textContent = `${formatCurrency(stopLossPrice)} (${(
            result.stopLossPercentage * 100
          ).toFixed(2)}%)`;

          document.getElementById("resultTradeDirection").textContent = result.tradeDirection;
          document.getElementById("resultAssetQuantity").textContent = `${result.assetQuantity} ${assetSymbol}`;
          document.getElementById("notionalValue").textContent = formatCurrency(result.notionalPositionValue);
          document.getElementById("marginRequired").textContent = `${formatCurrency(
            result.marginRequired
          )} (账户余额的 ${((result.marginRequired / accountBalance) * 100).toFixed(2)}%)`;

          document.getElementById("maxProfit").textContent = formatCurrency(result.maxProfit);
          document.getElementById("maxLoss").textContent = formatCurrency(result.maxLoss);
          document.getElementById("resultRiskRewardRatio").textContent = result.riskRewardRatio.toFixed(2);

          // 清除之前的警告信息
          document.getElementById("warningMessages").innerHTML = "";

          // 添加警告信息（如果有）
          if (!result.isRecommended) {
            const warningElement = document.createElement("div");
            warningElement.className = "warning-message";
            warningElement.innerHTML = "⛔ 警告: 盈亏比低于1.5，不建议交易!";
            document.getElementById("warningMessages").appendChild(warningElement);
          } else {
            const successElement = document.createElement("div");
            successElement.className = "success-message";
            successElement.innerHTML = "✅ 盈亏比大于1.5，交易可考虑";
            document.getElementById("warningMessages").appendChild(successElement);
          }

          if (!result.isSufficientBalance) {
            const warningElement = document.createElement("div");
            warningElement.className = "warning-message";
            warningElement.innerHTML = "⛔ 警告: 所需保证金超过账户余额!";
            document.getElementById("warningMessages").appendChild(warningElement);
          }

          // 滚动到结果部分
          document.getElementById("results").scrollIntoView({ behavior: "smooth" });
        } catch (error) {
          alert(`计算错误: ${error.message}`);
        }
      });
    </script>
  </body>
</html>
