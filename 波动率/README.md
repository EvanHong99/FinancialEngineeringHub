<meta charset="UTF-8">
<html>
<table>
    <thead>
    <tr>
        <th>标的</th>
        <th>任务类型</th>
        <th>link</th>
        <th>主要内容</th>
        <th>星级</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>隐波</td>
        <td>拟合</td>
        <td><a href="./隐波拟合/Deep Smoothing of the Implied Volatility Surface.pdf">Deep Smoothing of the Implied Volatility Surface.pdf</a></td>
        <td>
            核心思想：用神经网络输出修正系数，与Prior模型的输出相乘从而实现在符合基本规律的情况下对结果进行优化。类似于resnet。
           <ul>
                <li>- **文档主题**：介绍了一种利用神经网络（NN）拟合和预测隐含波动率曲面（IVS）的方法，该方法能够保证无套利机会，并且能够结合标准的IVS模型进行修正。</li>
                <li>- **文档背景**：说明了期权定价的重要性，以及标准的IVS模型的局限性，如无法灵活地复制市场价格和处理稀疏或错误的数据。</li>
                <li>- **文档贡献**：提出了一种新的方法，将总方差表示为一个神经网络和一个先验模型的乘积，并在损失函数中加入软约束来防止套利机会。先验模型可以是任何一个有效的总方差模型，如Black-Scholes模型或SSVI模型。神经网络则作为先验模型的修正器，提高了其复制观察到的市场价格的能力。软约束的设定是根据数理金融的理论结果来指导的。两个元素结合起来，可以构建一个逼真、灵活和简洁的IVS模型。并且在合成数据和真实市场数据上进行了效果评估和对比分析。</li>
                <li>- **实验结果**：使用不同的先验模型（BS，SSVI，Heston）和惩罚系数λ，对IVS进行拟合和预测，比较了不同模型的预测准确性和无套利性。结果显示，本文提出的方法在预测准确性和无套利性方面优于基准模型（Bates和SSVI模型）。</li>
                <li>- **附加结果**：在附录中展示了风险中性密度和局部波动率的图像，以及在苹果期权上的实验结果，显示了本文方法可以拟合复杂的IVS形状，如W形微笑。还讨论了使用IV差异加权的损失函数的效果和计算时间的问题。</li>
                <li>- **结论**：总结了本文的主要贡献，即提出了一种灵活的方法来以经济合理的方式定价金融衍生品。该方法通过使用多层神经网络建模IVS，并通过惩罚损失函数来塑造它。通过各种数值和实证应用验证了本文的方法。还讨论了本文方法的潜在扩展和改进方向。</li>
            </ul>
        </td>
        <td></td>
    </tr>
    <tr>
        <td>隐波</td>
        <td>拟合</td>
        <td><a href="./隐波拟合/A two-step framework for arbitrage-free prediction of the implied volatility surface.pdf">A two-step framework for arbitrage-free prediction of the implied volatility surface.pdf</a></td>
        <td>
            文献综述：
            <ul>
                <li>主流的方法有三类：Parametric models、splines、Machine learning models</li>
                <li>pca：PCA
 analysis, already explain most of the variations in their data;
 these eigenmodes are associated with the level, skewness, and
 convexity of the IVS</li>
            </ul>
            <ul>
                <li>- **文档主题**：本文研究了如何用无套利的方式预测和模拟隐含波动率曲面（IVS），并提出了一个两步框架。</li>
                <li>- **文档方法**：第一步，选择特征向量来表示IVS，并用长短期记忆模型（LSTM）来预测它们。第二步，用一个深度神经网络（DNN）模型，结合静态无套利约束，从预测的特征向量构造整个IVS。</li>
                <li>- **文档贡献**：本文的贡献有两方面。一是提供了一个通用的框架，可以在不引入静态套利的情况下预测和模拟IVS，这是现有方法所没有的特点。二是展示了如何构造IVS的特征，并在该框架下开发了一些成功的预测模型。</li>
                <li>- **文档数据**：本文使用了2009年1月1日至2020年12月31日的S&P500指数期权的IVS数据，共3021天，每天有374个观测点。</li>
                <li>- **无套利条件**：文档详细讨论了如何在实现深度神经网络（DNN）模型时，确保满足无套利条件。这些条件包括对于非常大的|m|值的σ2(m, τ)的限制行为。如果DNN模型经过足够数量的训练周期，那么在测试数据上的这些惩罚值将为零，这意味着模型几乎不会违反这些约束。</li>
                <li>- **模拟**：该框架也可以用来模拟隐含波动率表面（IVS）随时间的变化。这涉及到特征转换方程的编写，以及误差向量的计算。误差向量假设为均值为零且协方差矩阵为ε的独立同分布白噪声。</li>
                <li>- **实证结果**：文档提供了使用S&P 500指数期权的每日隐含波动率数据进行的实证结果。数据集被划分为训练集和测试集，其中包括了2020年由于COVID-19大流行引发的美国股市崩盘的测试期。</li>
                <li>- **特征提取**：文档详细讨论了三种特征提取方法的细节，并对每种方法的性能进行了比较。 特征提取部分的基础数据、特征提取方法以及最终的性能如下：
                    <ul>
                        - 基础数据：本文使用了从2009年1月1日到2020年12月31日的S&P500指数期权的隐含波动率曲面（IVS）数据，每天有374个不同的（δ, τ）对，其中δ是Black-Scholes delta，τ是剩余到期时间。由于本文将IVS视为m和τ的函数，其中m是对数正向货币性，因此需要将δ转换为m。最终，每天有一个154维的隐含波动率向量¯ t作为输入数据。
                        - 特征提取方法：本文考虑了三种方法来从隐含波动率数据中提取特征，分别是：
                    - **采样法（SAM）**：直接使用¯ t作为IVS的特征向量，不进行降维。这种方法的优点是能够更好地近似曲面，缺点是预测高维特征向量可能更困难。
                    - **主成分分析（PCA）**：参考Cont and Da Fonseca (2002)的方法，对¯ t的对数变化进行表面PCA，得到一组特征向量Zt，其维度为K，通常K远小于154。这种方法的优点是能够用少量的特征向量捕捉曲面的主要变化，缺点是基于线性组合的特征向量可能不够准确。
                    - **变分自编码器（VAE）**：参考Kingma and Welling (2013)的方法，使用一个编码器神经网络从¯ t中提取出一组潜在因子Zt，其维度为d，通常d远小于154。然后，使用一个解码器神经网络从Zt重构¯ t。这种方法的优点是能够提供一个灵活的非线性因子表示，缺点是需要训练两个神经网络。
                - 最终的性能：本文使用了长短期记忆（LSTM）模型来预测特征向量，然后使用一个深度神经网络（DNN）模型来从预测的特征向量构造无套利的IVS。本文使用了9.5年的数据来训练模型，并在2.5年的数据上进行了测试。本文发现，采样法和VAE方法在样本外的预测中表现最好，而PCA方法的误差几乎是前两者的三倍。这表明，基于PCA的预测方法不够准确。另一个重要的发现是，DNN模型在第二步中不仅能够消除静态套利，而且与标准的插值方法相比，能够显著降低预测误差。
                    </ul>
                </li>
                <li>- **模型训练**：文档详细描述了LSTM和DNN模型的训练过程，包括参数初始化、优化器的选择以及批量归一化的应用。</li>
                <li>- **模型比较**：文档比较了六种模型的性能，并进行了Diebold-Mariano (DM) 测试以评估预测性能的统计显著性。</li>
                <li>- **结论**：文档总结了研究结果，并提出了未来的研究方向。</li>
            </ul>
        </td>
        <td></td>
    </tr>
        <tr>
        <td>历史波动率</td>
        <td>calendar_effect</td>
        <td><a href="./历史波动率/holiday_or_calendar_effect/The High Holidays- Psychological mechanisms of honesty in real-life financial decisions.pdf">The High Holidays: Psychological mechanisms of honesty in real-life financial decisions</a></td>
        <td>
            <ul>
                <li>- **文档主题**：本文探讨了宗教、心理和金融市场之间的相互作用，特别是在犹太教的高节期间，人们对诚实的关注如何影响他们的投资决策。</li>
                <li>- **文档方法**：本文使用了不同的数据和模型，包括 VIX 和 VXO 作为隐含波动率的指标，以及实际波动率的估计。本文还考虑了季节性、其他金融因素和谷歌搜索量指数等变量的影响。</li>
                <li>- **文档结果**：本文发现， <strong>在高节期间，市场回报率异常低，隐含波动率和实际波动率异常高，而且隐含波动率超过了未来波动率的预期。</strong> 本文解释这些现象是由于高节期间人们对诚实的关注增强了他们的焦虑和自我反省，从而影响了他们的交易行为。</li>
                <li>- **文档贡献**：本文填补了实证研究中的一个空白，即使用真实的金融数据来检验诚实机制对投资者行为的影响。本文也提出了一个简单的交易策略，利用高节期间的波动率异常来获取超额收益。本文的发现对理解市场情绪、投资者心理和宗教信仰的作用有重要的启示。</li>
            </ul>
        </td>
        <td></td>
    </tr>
        <tr>
        <td>历史波动率</td>
        <td>calendar_effect</td>
        <td><a href="./历史波动率/holiday_or_calendar_effect/Calendar Effect in The Chinese Securities Market.pdf">Calendar Effect in The Chinese Securities Market.pdf</a></td>
        <td>
            <ul>
                <li>- **周日历效应**：中国期货市场、航运金融衍生品市场和上海黄金期货市场都存在周日历效应，即不同交易日的收益率和波动率有显著差异。其中，周一和周五的收益率和波动率较高，周二和周四的收益率较低，周三的波动率较大。</li>
                <li>- **信息传播影响**：周日历效应的存在与信息传播有关，例如国际期货市场的周五效应对中国期货市场的周一效应的影响，以及政府政策或上市公司公告对股指期货市场的影响。</li>
                <li>- **投资者行为影响**：周日历效应的存在也与投资者行为有关，例如投资者的风险厌恶策略、羊群效应、前景理论等，导致投资者在特定日期买卖金融衍生品，从而影响价格变动。</li>
            </ul>
        </td>
        <td></td>
    </tr>
        <tr>
        <td>隐波</td>
        <td>拟合</td>
        <td><a href="./VRP volatility risk premium/Implied volatility information of Chinese SSE 50 ETF options.pdf">Implied volatility information of Chinese SSE 50 ETF options.pdf</a></td>
        <td>
            VRPt = RVt − IVt
            <ul>
                <li>金融市场对未来波动率的预期高于实物波动率。The statistical results show that the means of volatility risk premiums of call options and put options are all negative according to moneyness and time to maturity, indicating that China's financial marketexpectation of future volatility is always higher than the physical volatility. China's GDP has been rising at high rate every year, and the financial market has shown an overall upward trend and occasional sharp corrections, which have led to the phenomenon of large fluctuations in China's financial market. Therefore, China's financial market has a high expectation for future volatility, which tends to exceed the physical volatility of the current financial market.</li>
                <li>We divided the options sample into call options and put options. The regression coefficients of call and put options are both significantly positive, indicating that the volatility risk premium positively affects the realized volatility of the underlying security. Economic uncertainty in markets increases when volatility risk premiums is higher. Investors will panic in the face of possible extreme risk of loss, which in turn will increase trading volume and ultimately increase the volatility of the underlying securities.
                    我们将期权样本分为看涨期权和看跌期权。看涨期权和看跌期权的回归系数均显著为正，表明波动率风险溢价对标的证券的已实现波动率有正向影响。当波动性风险溢价较高时，市场的经济不确定性就会增加。面对可能出现的极端损失风险，投资者会感到恐慌，这反过来又会增加交易量，最终增加相关证券的波动性。</li>
            </ul>
        </td>
        <td></td>
    </tr>
    <tr>
        <td>隐波</td>
        <td>拟合</td>
        <td><a href="./VRP volatility risk premium/Dynamic estimation of volatility risk premia and investor risk aversion from option-implied and realized volatilities.pdf">Dynamic estimation of volatility risk premia and investor risk aversion from option-implied and realized volatilities.pdf</a></td>
        <td>
            <ul>
                <li>提出了一种Model-free implied volatility计算方式</li>
                <li>给出了如何计算rv的公式</li>
                <li>如何计算iv</li>
                <li>如何评价波动率</li>
                <li>This paper develops a simple consistent approach for estimating
the volatility risk premium. The approach exploits the linkage
between the objective and risk-neutral expectations of the
integrated volatility. The estimation is facilitated by the use of
newly available model-free realized volatilities based on highfrequency intraday data along with model-free option-implied
volatilities.</li>
            </ul>
        </td>
        <td></td>
    </tr>
    <tr>
        <td>隐波</td>
        <td>拟合</td>
        <td><a href="./VRP volatility risk premium/Implied volatility information of Chinese SSE 50 ETF options.pdf">Implied volatility information of Chinese SSE 50 ETF options</a></td>
        <td>
            <ul>
                <li>提出了一种Model-free implied volatility计算方式</li>
                <li>给出了如何计算VRP的公式: 1. stochastic volatility model 反推  (Bakshi, 2003; Duan & Yeh, 2010; Neumann, Prokopczuk, &
                    Simen, 2016; Bardgett, Gourier, & Leippold, 2019) 2. 通过variance swap来计算 ( Carr and Wu (2009))： <math>EtQ(RVt) = SWt = Et P(mtRVt) = Et P(RVt) + COVt P(mt, RVt)</math></li>
            </ul>
        </td>
        <td></td>
    </tr>
    </tbody>
</table>
</html>
<!--
    <tr>
        <td>隐波</td>
        <td>拟合</td>
        <td><a href="./历史波动率/"></a></td>
        <td>
            <ul>
                <li></li>
            </ul>
        </td>
        <td></td>
    </tr>
    <strong>.</strong>
-->