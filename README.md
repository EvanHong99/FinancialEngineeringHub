# 研报内容摘要及阅读体会

[//]: # (基本面，择时，因子，组合优化)


<!-- ===============开始=============== -->

[//]: # (<table>)

[//]: # (    <thead>)

[//]: # (    <tr>)

[//]: # (        <th>领域</th>)

[//]: # (        <th>主题</th>)

[//]: # (        <th>link</th>)

[//]: # (        <th>主要内容</th>)

[//]: # (        <th>星级</th>)

[//]: # (    </tr>)

[//]: # (    </thead>)

[//]: # (    <tbody>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>介绍</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/海通证券_听海外高频交易专家讲解美国的高频交易.pdf">海通证券_听海外高频交易专家讲解美国的高频交易.pdf</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>介绍flash crash“闪崩”，由于交易者（包括做市商）不愿承接大卖单，委买数量急剧下降，流动性枯竭，导致市场快速下跌<br/>)

[//]: # (                </li>)

[//]: # (                <li>介绍了逆向选择（Adverse)

[//]: # (                    Selection）它对高频交易的成功实施至关重要，可以说，任何一次高频交易本质上都是为了尽可能地避免被逆向选择。一般认为，越靠近最新形成的价格的委托单（价格优先时间优先），遭遇的逆向选择越少。<br/>)

[//]: # (                </li>)

[//]: # (                <li>“Hide not Slide”委买单</li>)

[//]: # (                <li>当前业界知名且业绩优异的高频交易公司大约有十几家。有些以速度见长，比如前文提到的Virtu；有些在基于订单簿的信号研究上非常突出，比如Citadel、Two)

[//]: # (                    Sigma。 据了解，Citadel 80%的交易都是以拿单（消耗市场流动性）的方式完成的，这就说明他 们有着非常强大的趋势预测能力)

[//]: # (                </li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td>1</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>介绍</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/平安证券_策略专题报告_从海外经验看中国高频交易的发展.pdf">平安证券_策略专题报告：从海外经验看中国高频交易的发展.pdf</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>介绍了美国高频、中国高频发展</li>)

[//]: # (                <li>高频交易的主要投资策略<br>)

[//]: # (                    <ul>)

[//]: # (                        <li>被动做市交易策略：介绍了做市的具体操作和逻辑</li>)

[//]: # (                        <li>结构性策略：结构性策略是挃交易者利用不公平的交易机制获利</li>)

[//]: # (                        <li>方向性策略</li>)

[//]: # (                        <li>套利策略</li>)

[//]: # (                    </ul>)

[//]: # (                </li>)

[//]: # (                <li><strong>介绍了美国的监管制度</strong></li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td>2</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>因子-spread tick / spread date / BuyRate</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/2019-09-05_天风证券_市场微观结构探析系列之二：订单簿上的alpha.pdf">2019-09-05_天风证券_市场微观结构探析系列之二：订单簿上的alpha</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            通过高频spread tick因子计算spread date/month，有显著盈利能力。且和BuyRate负相关性)

[//]: # (        </td>)

[//]: # (        <td>2</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>因子</td>)

[//]: # (        <td><a href="https://zhuanlan.zhihu.com/p/138926388">博客-《【高频】Level-2高频数据的实证研究（一）》</a></td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>介绍了多个因子及其出处</li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td>3</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>因子-order imbalance</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://bigquant.com/wiki/pdfjs/web/viewer.html?file=/wiki/static/upload/2b/2bc961b3-e365-4afb-aa98-e9f9d9fa299e.pdf">天风证券_买卖压力失衡——利用高频数据拓展盘口数据</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>买卖压力比</li>)

[//]: # (                <li>计算个股历史买卖压力分布，取1.96标准差为阈值，超过阈值则为买/卖压占优</li>)

[//]: # (                <li>)

[//]: # (                    买卖压力失衡情况消失后，股票的超额收益呈现反向逆转，这意味着买卖压力失衡带来的超额收益仅仅为短期冲击影响，后期股价会逐步修正恢复到原状态。)

[//]: # (                </li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td>2</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>因子-order imbalance</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/牛津教材Order Imbalance Based Strategy in High Frequency Trading.pdf">牛津教材Order)

[//]: # (                Imbalance Based Strategy in High Frequency Trading</a></td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>Volume Order Imbalance &#40;VOI&#41;</li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td>3</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>因子-order imbalance</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/Cao, C. The information content of an open limit‐order book.pdf">THE)

[//]: # (                INFORMATION CONTENT OF AN OPEN LIMIT-ORDER BOOK. CHARLES CAO etc.</a></td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li></li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td></td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>因子-大单分析</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/2020-06-22_海通证券_选股因子系列研究（六十六）：寻找逐笔交易中的有效信息.pdf">2020-06-22_海通证券_选股因子系列研究（六十六）：寻找逐笔交易中的有效信息</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>基于逐笔信息的大买成交金额占比：买单或者卖单为大单的所有成交金额占全天 成交额比例。</li>)

[//]: # (                <li>通过对于大单因子选股特性的 细致分析，我们可以发现只要大额买单成交占比较高，则未来股票较大概率跑赢)

[//]: # (                    市场。然而大额卖单占比较高时，如果其成交对手方也是大资金方，则其对于未 来股票走势预测能力非常微弱。)

[//]: # (                </li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td></td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>预测-分类-Price jump</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/Price jump prediction in Limit Order Book.pdf">Price)

[//]: # (                jump prediction in Limit Order Book.pdf</a></td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>因子：1. Bid-Ask volume ratio；2.根据订单簿事件构建的dummies</li>)

[//]: # (                <li>超短期预测，分类</li>)

[//]: # (                <li>lasso&#40;variable selection&#41;+logistic&#40;prediction&#41;</li>)

[//]: # (                <li>结果还行，0.7+的AUC</li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td>3</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>预测-回归/分类-3 directions</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/THE SHORT-TERM PREDICTABILITY OF RETURNS IN ORDER BOOK MARKETS A DEEP LEARNING PERSPECTIVE.pdf">THE)

[//]: # (                SHORT-TERM PREDICTABILITY OF RETURNS IN ORDER BOOK MARKETS A DEEP LEARNING PERSPECTIVE.pdf</a>)

[//]: # (            ...<a href="https://github.com/lorenzolucchese/deepOBs">github</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            <ul>)

[//]: # (                <li>LOB数据来源（免费）：<a href="https://lobsterdata.com/"><b>LOBSTER.</b>使用原始数据进行预测（10档price)

[//]: # (                    and)

[//]: # (                    volume），对源数据进行10个订单簿事件的上采样（文章未明确指出，但应该是指new)

[//]: # (                    limit order事件、trade-through成交事件、cancel order事件）。</a></li>)

[//]: # (                <li>文章强调了进行相关研究应该遵循的robust规则<a)

[//]: # (                        href="https://ideas.repec.org/p/arx/papers/2110.05479.html">Towards Robust Representation of)

[//]: # (                    Limit Orders Books for Deep Learning Models</a></li>)

[//]: # (                <li>预测target：<a href="./imgs/高频/8.png">avg_mid_price_ret</a></li>)

[//]: # (                <li>本文主要对以下模型进行了分析和对比，并使用<b>model confidence set&#40;MCS&#41; 来衡量预测可信度</b>)

[//]: # (                    <ol>)

[//]: # (                        <li>)

[//]: # (                            <a href="https://ieeexplore.ieee.org/document/8673598/">DeepLOB: Deep Convolutional Neural)

[//]: # (                                Networks for Limit Order Books</a>...click)

[//]: # (                            for structure<a href="./imgs/高频/1.png">[1]</a><a href="./imgs/高频/2.png">[2]</a><a)

[//]: # (                                href="./imgs/高频/3.png">[3]</a>.)

[//]: # (                            <ol>)

[//]: # (                                <li>使用raw data</li>)

[//]: # (                                <li>CNN: aggregate information across order book levels, and the temporal convolutions)

[//]: # (                                    can)

[//]: # (                                    be)

[//]: # (                                    understood as smoothing operations)

[//]: # (                                </li>)

[//]: # (                                <li>Inception module: 1d-convolution, can be interpreted as a &#40;weighted&#41;)

[//]: # (                                    moving average.)

[//]: # (                                </li>)

[//]: # (                                <li>LSTM: longer-term dependencies</li>)

[//]: # (                            </ol>)

[//]: # (                        </li>)

[//]: # (                        <li>)

[//]: # (                            <a href="">DeepOF: Deep Order Flow Imbalance: Extracting Alpha at Multiple Horizons from the)

[//]: # (                                Limit Order Book</a>...click for structure<a href="./imgs/高频/4.png">[1]</a>.)

[//]: # (                            <ol>)

[//]: # (                                <li>使用derived quantity, order flow.</li>)

[//]: # (                            </ol>)

[//]: # (                        </li>)

[//]: # (                        <li>)

[//]: # (                            DeepVOL: 根据上文提到的规范，提出DeepVOL<a href="./imgs/高频/5.png">[1]</a>)

[//]: # (                            <ol>)

[//]: # (                                <li>解决前两个模型不够完善的可解释性、规范性、目的性</li>)

[//]: # (                                <li>提高了模型可复用性，仍旧使用DeepLOB作为backend模型</li>)

[//]: # (                                <li>对数据的表示方式进行修改，因此需要增加CNN进行DeepLOB适配</li>)

[//]: # (                                <li>增加使用L3数据，将逐笔委托的大小也纳入考量，利用CNN计算相应特征喂到DeepLOB</li>)

[//]: # (                            </ol>)

[//]: # (                        </li>)

[//]: # (                        <li>)

[//]: # (                            Multi-horizon models: 在前面的基础上，保证robustness以及利用了L3数据，借鉴NLP翻译的思想（seq2seq）提出Multi-horizon)

[//]: # (                            models.<a)

[//]: # (                                href="./imgs/高频/7.png">[1]</a>)

[//]: # (                            <a)

[//]: # (                                    href="https://ideas.repec.org/p/arx/papers/2105.10430.html">Multi-Horizon)

[//]: # (                                Forecasting for Limit Order Books: Novel Deep Learning Approaches)

[//]: # (                                and Hardware Acceleration using Intelligent Processing Units</a>)

[//]: # (                            <ol>)

[//]: # (                                <li>借鉴NLP的思想（sequence to sequence，比如翻译任务），使用RNN based/RNN+attention)

[//]: # (                                    based/transformer&#40;only)

[//]: # (                                    attention&#41; based encoder-decoder)

[//]: # (                                    models，预测不再是一个终值，而是序列<a href="./imgs/高频/6.png">[1]</a></li>)

[//]: # (                            </ol>)

[//]: # (                            回忆<a)

[//]: # (                                href="https://lena-voita.github.io/nlp_course/seq2seq_and_attention.html">[全部知识回顾5++]</a>：embedding、attention结构、end-to-end、transformer、self-attention<a)

[//]: # (                                href="https://lena-voita.github.io/nlp_course/seq2seq_and_attention.html#:~:text=Self%2DAttention%3A%20the%20%22Look%20at%20Each%20Other%22%20Part">[1]</a>)

[//]: # (                        </li>)

[//]: # (                    </ol>)

[//]: # (                </li>)

[//]: # (                <li>)

[//]: # (                    结论)

[//]: # (                    <ol>)

[//]: # (                        <li>Q: Do high frequency returns display predictability? If so, how far ahead can we)

[//]: # (                            predict?<br>)

[//]: # (                            A: we were able to identify predictability up to 50 order book events ahead at the 99%)

[//]: # (                            confidence level.)

[//]: # (                        </li>)

[//]: # (                        <li>Q: Which order book representations perform the best?<br>)

[//]: # (                            A: L1->L2 greatly improves the performance, L2->L3 does not seem to provide a clear)

[//]: # (                            advantage: deepVOL&#40;L2&#41; and deepVOL&#40;L3&#41; display similar performance.)

[//]: # (                        </li>)

[//]: # (                        <li>Q: Can we use a single model across multiple horizons?<br>)

[//]: # (                            A: 使用seq2seq可以大幅提升模型在不同预测steps（horizons）下的表现)

[//]: # (                        </li>)

[//]: # (                        <li>Q: Can we use a single model across multiple stocks?<br>)

[//]: # (                            A: 和别人文章不同<a href="https://doi.org/10.1080/14697688.2019.1622295">[1)

[//]: # (                                ]</a>，不同股票有不同交易pattern。即使是在和train同源的valid集上，不同in-sample股票的预测能力也差别巨大，如AAPL就不能很好地在valid)

[//]: # (                            上预测，其余out-of-sample股票的预测更是困难。<br>)

[//]: # (                        </li>)

[//]: # (                    </ol>)

[//]: # (                </li>)

[//]: # (            </ul>)

[//]: # (            <a href="https://arxiv.org/pdf/1803.01271.pdf">补充资料：时序卷积网络TCN-Temporal Convolutional)

[//]: # (                Network</a><br>)

[//]: # (            <a href="https://github.com/unit8co/darts">python包</a><br>)

[//]: # (            <b>todo: Attention</b>)

[//]: # (        </td>)

[//]: # (        <td>5+</td>)

[//]: # (    </tr>)

[//]: # (    <tr>)

[//]: # (        <td>高频</td>)

[//]: # (        <td>预测-回归-股票波动性</td>)

[//]: # (        <td>)

[//]: # (            <a href="https://www.kaggle.com/competitions/optiver-realized-volatility-prediction">kaggle optiver</a><br>)

[//]: # (            <a href="https://mp.weixin.qq.com/s/Pe4i3I9-ErYFE9uL5B5pvQ">金牌思想</a>)

[//]: # (        </td>)

[//]: # (        <td>)

[//]: # (            target: 应用前10分钟的Book和Trade数据预测下个10分钟的已实现波动率。<br>)

[//]: # (            <b>特征工程：和我之前做法不同的是，他并没有采用将原始数据进行shift+右连接，而是使用一些aggregate函数（如avg、std、min、max）进行下采样</b>)

[//]: # (            <ul>)

[//]: # (                <li>)

[//]: # (                    "log_return"/"log_return2"：计算的是每个time_id内相邻两个快照的收益率，没两个快照之间的时间间隔可能不一致，如示例数据中的秒数间隔数为1、4、1、1。)

[//]: # (                </li>)

[//]: # (                <li>)

[//]: # (                    "wap_balance"/"price_spread"/"volume_imbalance"等等（代码21-27行所示）：计算的是这个time_id内这个特征在这个时间段内的平均值。如果自己尝试时，也可以增加其他统计维度的值，如最大最小，标准差等。)

[//]: # (                </li>)

[//]: # (                <li>对个股进行dummy，但是不是one-hot，而是采用其train上的平均ret作为识别id，因此不需要get_dummies转为一个matrix，只需要一个numerical)

[//]: # (                    series)

[//]: # (                    就能表示)

[//]: # (                </li>)

[//]: # (            </ul>)

[//]: # (        </td>)

[//]: # (        <td></td>)

[//]: # (    </tr>)

[//]: # (    </tbody>)

[//]: # (</table>)


<!--
    <tr>
        <td></td>
        <td></td>
        <td><a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/"></a></td>
        <td>
            <ul>
                <li></li>
            </ul>
        </td>
        <td></td>
    </tr>

    <strong>.</strong>
-->


<!-- ================结束================ -->



<!--
        <tr>
            <td></td>
            <td></td>
            <td><a href="https://github.com/EvanHong99/FinancialEngineeringHub/blob/master/高频/订单簿lob/"></a></td>
            <td>
                <ol>
                    <li></li>
                </ol>
            </td>
            <td></td>
        </tr>

    <strong>.</strong>
-->
