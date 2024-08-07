# Test Coverage

The tables below provides a summary and detailed information in relation to the number of tests performed, the count of passing tests and the count of failing tests.

To summarize, VeChain achieves a pass rate of 99%, when taking into consideration that 1346 of the 1355 failing tests are classified as being either justifiable or passable, given some modifications to the tests.

You can find detailed analysis of the coverage categories in the pages to follow.

### Summary Table (Oz4)
<table><thead><tr><th width="307">Category</th><th width="399.3333333333333">Short Description</th><th>Failures</th></tr></thead><tbody><tr><td>Justifiable</td><td>Failures that result from the inherent design differences between VeChain and Ethereum.</td><td>73</td></tr><tr><td>Contract Address Prediction</td><td>See <a href="https://github.com/vechain/vechain-docs/blob/main/core-concepts/evm-compatibility/test-coverage/broken-reference/README.md">here</a>.</td><td>14</td></tr><tr><td>Failures in Constructor</td><td>Contract fails in constructor resulting in failure to be deployed.</td><td>7</td></tr><tr><td>Full, with eth_sign implementation</td><td>See <a href="https://github.com/vechain/vechain-docs/blob/main/core-concepts/evm-compatibility/test-coverage/broken-reference/README.md">here</a>.</td><td>4</td></tr><tr><td>Full, with test changes</td><td>Some test modifications had to be added for the tests to pass.</td><td>3</td></tr><tr><td>BadBeaconProxy Address 0x1</td><td>See <a href="https://github.com/vechain/vechain-docs/blob/main/core-concepts/evm-compatibility/test-coverage/broken-reference/README.md">here</a>.</td><td>1</td></tr></tbody></table>

### Summary Table (Oz5 Shanghai)
<table>
    <thead>
        <tr>
            <th width="307">Category</th>
            <th width="399.3333333333333">Short Description</th>
            <th>Failures</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Justifiable</td>
            <td>Failures that result from the inherent design differences between VeChain and Ethereum.</td>
            <td>83</td>
        </tr>
        <tr>
            <td>Custom Error</td>
            <td>Failures due to custom errors specific to the implementation.</td>
            <td>928</td>
        </tr>
        <tr>
            <td>Hardhat Specific</td>
            <td>Issues specific to Hardhat Network.</td>
            <td>335</td>
        </tr>
        <tr>
            <td>Max code size limit</td>
            <td>Failures due to exceeding the maximum contract code size limit.</td>
            <td>4</td>
        </tr>
        <tr>
            <td>BadBeaconProxy Address 0x1</td>
            <td>See <a href="https://github.com/vechain/vechain-docs/blob/main/core-concepts/evm-compatibility/test-coverage/broken-reference/README.md">here</a></td>
            <td>1</td>
        </tr>
        <tr>
            <td>eth_sign</td>
            <td>See <a href="https://docs.vechain.org/core-concepts/evm-compatibility/test-coverage/eth_sign">here</a>.</td>
            <td>4</td>
        </tr>
    </tbody>
</table>


### Detailed Table (Oz4)
<table><thead><tr><th width="309">Contract Name</th><th width="241">Test Coverage</th><th width="94">Pass</th><th width="104">Fail</th><th>Total</th><th data-hidden>Hardhat Total Tests</th></tr></thead><tbody><tr><td><strong>Total</strong></td><td></td><td><strong>2324</strong></td><td><strong>102</strong></td><td><strong>2426</strong></td><td><strong>2667</strong></td></tr><tr><td>ERC1967Proxy</td><td></td><td>25</td><td>3</td><td>28</td><td>28</td></tr><tr><td>TransparentUpgradeableProxy</td><td></td><td>58</td><td>3</td><td>61</td><td>61</td></tr><tr><td>BeaconProxy</td><td></td><td>7</td><td>2</td><td>9</td><td>9</td></tr><tr><td>GovernorTimelockCompound</td><td></td><td>7</td><td>12</td><td>19</td><td>19</td></tr><tr><td>GovernorCompatibilityBravo</td><td></td><td>7</td><td>2</td><td>9</td><td>9</td></tr><tr><td>TimelockController</td><td></td><td>27</td><td>15</td><td>42</td><td>48</td></tr><tr><td>CrossChainEnabled</td><td></td><td>4</td><td>9</td><td>13</td><td>15</td></tr><tr><td>GovernorTimelockControl</td><td></td><td>12</td><td>9</td><td>21</td><td>21</td></tr><tr><td>AccessControl</td><td></td><td>50</td><td>4</td><td>54</td><td>80</td></tr><tr><td>MinimalForwarder</td><td></td><td>12</td><td>4</td><td>16</td><td>15</td></tr><tr><td>TokenTimelock</td><td></td><td>3</td><td>4</td><td>7</td><td>7</td></tr><tr><td>VestingWallet</td><td></td><td>2</td><td>4</td><td>6</td><td>6</td></tr><tr><td>ERC721Enumerable</td><td></td><td>233</td><td>3</td><td>236</td><td>236</td></tr><tr><td>DoubleEndedQueue</td><td></td><td>7</td><td>2</td><td>9</td><td>9</td></tr><tr><td>ERC2771Context</td><td></td><td>5</td><td>2</td><td>7</td><td>7</td></tr><tr><td>ERC721</td><td></td><td>211</td><td>2</td><td>213</td><td>213</td></tr><tr><td>Governor</td><td></td><td>42</td><td>2</td><td>44</td><td>44</td></tr><tr><td>Checkpoints</td><td></td><td>22</td><td>1</td><td>23</td><td>23</td></tr><tr><td>ERC1155</td><td></td><td>83</td><td>1</td><td>84</td><td>84</td></tr><tr><td>ERC1155Holder</td><td></td><td>4</td><td>1</td><td>5</td><td>5</td></tr><tr><td>ERC1155PresetMinterPauser</td><td></td><td>16</td><td>1</td><td>17</td><td>17</td></tr><tr><td>ERC165</td><td></td><td>2</td><td>1</td><td>3</td><td>3</td></tr><tr><td>ERC165Storage</td><td></td><td>4</td><td>1</td><td>5</td><td>5</td></tr><tr><td>ERC20Votes</td><td></td><td>28</td><td>1</td><td>29</td><td>29</td></tr><tr><td>ERC20VotesComp</td><td></td><td>27</td><td>1</td><td>28</td><td>28</td></tr><tr><td>ERC721PresetMinterPauserAutoId</td><td></td><td>15</td><td>1</td><td>16</td><td>16</td></tr><tr><td>ERC721Royalty</td><td></td><td>13</td><td>1</td><td>14</td><td>14</td></tr><tr><td>GovernorWithParams</td><td></td><td>3</td><td>1</td><td>4</td><td>4</td></tr><tr><td>MerkleProof</td><td></td><td>8</td><td>1</td><td>9</td><td>9</td></tr><tr><td>TimersTimestamp</td><td></td><td>4</td><td>1</td><td>5</td><td>5</td></tr><tr><td>ECDSA</td><td></td><td>14</td><td>3</td><td>17</td><td>17</td></tr><tr><td>SignatureChecker (ERC1271)</td><td></td><td>1</td><td>1</td><td>1</td><td>7</td></tr><tr><td>ERC1820Implementer</td><td></td><td>1</td><td>1</td><td>1</td><td>6</td></tr><tr><td>ERC777</td><td></td><td>1</td><td>1</td><td>1</td><td>193</td></tr><tr><td>ERC777PresetFixedSupply</td><td></td><td>1</td><td>1</td><td>1</td><td>6</td></tr><tr><td>Address</td><td></td><td>29</td><td>0</td><td>29</td><td>29</td></tr><tr><td>Arrays</td><td></td><td>15</td><td>0</td><td>15</td><td>15</td></tr><tr><td>BitMap</td><td></td><td>10</td><td>0</td><td>10</td><td>10</td></tr><tr><td>Clones</td><td></td><td>30</td><td>0</td><td>30</td><td>30</td></tr><tr><td>ConditionalEscrow</td><td></td><td>11</td><td>0</td><td>11</td><td>11</td></tr><tr><td>Context</td><td></td><td>4</td><td>0</td><td>4</td><td>4</td></tr><tr><td>Counters</td><td></td><td>8</td><td>0</td><td>8</td><td>8</td></tr><tr><td>Create2</td><td></td><td>8</td><td>0</td><td>8</td><td>8</td></tr><tr><td>EIP712</td><td></td><td>2</td><td>0</td><td>2</td><td>2</td></tr><tr><td>EnumerableMap</td><td></td><td>70</td><td>0</td><td>70</td><td>70</td></tr><tr><td>EnumerableSet</td><td></td><td>20</td><td>0</td><td>24</td><td>24</td></tr><tr><td>ERC1155Burnable</td><td></td><td>6</td><td>0</td><td>6</td><td>6</td></tr><tr><td>ERC1155Pausable</td><td></td><td>11</td><td>0</td><td>11</td><td>11</td></tr><tr><td>ERC1155Supply</td><td></td><td>10</td><td>0</td><td>10</td><td>10</td></tr><tr><td>ERC1155URIStorage</td><td></td><td>4</td><td>0</td><td>4</td><td>4</td></tr><tr><td>ERC165Checker</td><td></td><td>40</td><td>0</td><td>40</td><td>40</td></tr><tr><td>ERC20</td><td></td><td>118</td><td>0</td><td>118</td><td>118</td></tr><tr><td>ERC20Burnable</td><td></td><td>13</td><td>0</td><td>13</td><td>13</td></tr><tr><td>ERC20Capped</td><td></td><td>5</td><td>0</td><td>5</td><td>5</td></tr><tr><td>ERC20FlashMint</td><td></td><td>12</td><td>0</td><td>12</td><td>12</td></tr><tr><td>ERC20Pausable</td><td></td><td>12</td><td>0</td><td>12</td><td>12</td></tr><tr><td>ERC20Permit</td><td></td><td>6</td><td>0</td><td>6</td><td>6</td></tr><tr><td>ERC20PresetFixedSupply</td><td></td><td>4</td><td>0</td><td>4</td><td>4</td></tr><tr><td>ERC20PresetMinterPauser</td><td></td><td>12</td><td>0</td><td>12</td><td>12</td></tr><tr><td>ERC20Snapshot</td><td></td><td>14</td><td>0</td><td>14</td><td>14</td></tr><tr><td>ERC4626</td><td></td><td>25</td><td>0</td><td>25</td><td>25</td></tr><tr><td>ERC721Burnable</td><td></td><td>4</td><td>0</td><td>4</td><td>4</td></tr><tr><td>ERC721Consecutive</td><td></td><td>13</td><td>0</td><td>13</td><td>13</td></tr><tr><td>ERC721Holder</td><td></td><td>1</td><td>0</td><td>1</td><td>1</td></tr><tr><td>ERC721Pausable</td><td></td><td>10</td><td>0</td><td>10</td><td>10</td></tr><tr><td>ERC721URIStorage</td><td></td><td>10</td><td>0</td><td>10</td><td>10</td></tr><tr><td>ERC721Votes</td><td></td><td>26</td><td>0</td><td>26</td><td>26</td></tr><tr><td>Escrow</td><td></td><td>10</td><td>0</td><td>10</td><td>10</td></tr><tr><td>GovernorComp</td><td></td><td>2</td><td>0</td><td>2</td><td>2</td></tr><tr><td>GovernorERC721Mock</td><td></td><td>2</td><td>0</td><td>2</td><td>2</td></tr><tr><td>GovernorPreventLateQuorum</td><td></td><td>5</td><td>0</td><td>5</td><td>5</td></tr><tr><td>GovernorVotesQuorumFraction</td><td></td><td>6</td><td>0</td><td>6</td><td>6</td></tr><tr><td>Initializable</td><td></td><td>29</td><td>0</td><td>29</td><td>29</td></tr><tr><td>Math</td><td></td><td>25</td><td>0</td><td>25</td><td>25</td></tr><tr><td>MulticallToken</td><td></td><td>4</td><td>0</td><td>4</td><td>4</td></tr><tr><td>Ownable</td><td></td><td>6</td><td>0</td><td>6</td><td>6</td></tr><tr><td>Ownable2Step</td><td></td><td>5</td><td>0</td><td>5</td><td>5</td></tr><tr><td>Pausable</td><td></td><td>11</td><td>0</td><td>11</td><td>11</td></tr><tr><td>PaymentSplitter</td><td></td><td>20</td><td>0</td><td>20</td><td>20</td></tr><tr><td>ProxyAdmin</td><td></td><td>12</td><td>0</td><td>12</td><td>12</td></tr><tr><td>PullPayment</td><td></td><td>4</td><td>0</td><td>4</td><td>4</td></tr><tr><td>ReentrancyGuard</td><td></td><td>6</td><td>0</td><td>6</td><td>6</td></tr><tr><td>RefundEscrow</td><td></td><td>17</td><td>0</td><td>17</td><td>17</td></tr><tr><td>SafeCast</td><td></td><td>444</td><td>0</td><td>444</td><td>444</td></tr><tr><td>SafeERC20</td><td></td><td>35</td><td>0</td><td>35</td><td>35</td></tr><tr><td>SafeMath</td><td></td><td>48</td><td>0</td><td>48</td><td>48</td></tr><tr><td>SignedMath</td><td></td><td>12</td><td>0</td><td>12</td><td>12</td></tr><tr><td>SignedSafeMath</td><td></td><td>17</td><td>0</td><td>17</td><td>17</td></tr><tr><td>StorageSlot</td><td></td><td>12</td><td>0</td><td>12</td><td>12</td></tr><tr><td>Strings</td><td></td><td>31</td><td>0</td><td>31</td><td>31</td></tr><tr><td>TimersBlockNumber</td><td></td><td>5</td><td>0</td><td>5</td><td>5</td></tr><tr><td>UpgradeableBeacon</td><td></td><td>5</td><td>0</td><td>5</td><td>5</td></tr><tr><td>UUPSUpgradeable</td><td></td><td>6</td><td>0</td><td>6</td><td>6</td></tr><tr><td>Votes</td><td></td><td>23</td><td>0</td><td>23</td><td>23</td></tr></tbody></table>

### Detailed Table (Oz5 Shanghai)
<table>
  <thead>
    <tr>
      <th width="309">Contract Name</th>
      <th width="241">Test Coverage</th>
      <th width="94">Pass</th>
      <th width="104">Fail</th>
      <th>Total</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>AccessControl</td><td></td><td>30</td><td>9</td><td>39</td><td></td></tr>
    <tr><td>Ownable</td><td></td><td>8</td><td>4</td><td>12</td><td></td></tr>
    <tr><td>Ownable2Step</td><td></td><td>6</td><td>2</td><td>8</td><td></td></tr>
    <tr><td>AccessControlDefaultAdminRules</td><td></td><td>94</td><td>67</td><td>161</td><td></td></tr>
    <tr><td>AccessControlEnumerable</td><td></td><td>37</td><td>11</td><td>48</td><td></td></tr>
    <tr><td>AccessManaged</td><td></td><td>11</td><td>6</td><td>17</td><td></td></tr>
    <tr><td>AccessManager</td><td></td><td>160</td><td>185</td><td>345</td><td></td></tr>
    <tr><td>AuthorityUtils</td><td></td><td>4</td><td>0</td><td>4</td><td></td></tr>
    <tr><td>VestingWallet</td><td></td><td>6</td><td>5</td><td>11</td><td></td></tr>
    <tr><td>Governor</td><td></td><td>202</td><td>143</td><td>345</td><td></td></tr>
    <tr><td>TimelockController</td><td></td><td>53</td><td>38</td><td>91</td><td></td></tr>
    <tr><td>GovernorERC721</td><td></td><td>4</td><td>2</td><td>6</td><td></td></tr>
    <tr><td>GovernorPreventLateQuorum</td><td></td><td>10</td><td>7</td><td>17</td><td></td></tr>
    <tr><td>GovernorTimelockCompound</td><td></td><td>38</td><td>36</td><td>74</td><td></td></tr>
    <tr><td>GovernorTimelockControl</td><td></td><td>42</td><td>37</td><td>79</td><td></td></tr>
    <tr><td>GovernorVotesQuorumFraction</td><td></td><td>12</td><td>10</td><td>22</td><td></td></tr>
    <tr><td>GovernorWithParams</td><td></td><td>14</td><td>11</td><td>25</td><td></td></tr>
    <tr><td>Votes</td><td></td><td>46</td><td>14</td><td>60</td><td></td></tr>
    <tr><td>ERC2771Context</td><td></td><td>11</td><td>0</td><td>11</td><td></td></tr>
    <tr><td>ERC2771Forwarder</td><td></td><td>37</td><td>19</td><td>56</td><td></td></tr>
    <tr><td>Clones</td><td></td><td>30</td><td>1</td><td>31</td><td></td></tr>
    <tr><td>ERC1967Proxy</td><td></td><td>26</td><td>12</td><td>38</td><td></td></tr>
    <tr><td>BeaconProxy</td><td></td><td>10</td><td>8</td><td>18</td><td></td></tr>
    <tr><td>UpgradeableBeacon</td><td></td><td>6</td><td>3</td><td>9</td><td></td></tr>
    <tr><td>ProxyAdmin</td><td></td><td>7</td><td>4</td><td>11</td><td></td></tr>
    <tr><td>TransparentUpgradeableProxy</td><td></td><td>26</td><td>12</td><td>38</td><td></td></tr>
    <tr><td>Initializable</td><td></td><td>29</td><td>8</td><td>37</td><td></td></tr>
    <tr><td>UUPSUpgradeable</td><td></td><td>11</td><td>10</td><td>21</td><td></td></tr>
    <tr><td>ERC1155</td><td></td><td>89</td><td>29</td><td>118</td><td></td></tr>
    <tr><td>ERC1155Burnable</td><td></td><td>6</td><td>2</td><td>8</td><td></td></tr>
    <tr><td>ERC1155Pausable</td><td></td><td>11</td><td>8</td><td>19</td><td></td></tr>
    <tr><td>ERC1155Supply</td><td></td><td>11</td><td>0</td><td>11</td><td></td></tr>
    <tr><td>ERC1155URIStorage</td><td></td><td>4</td><td>0</td><td>4</td><td></td></tr>
    <tr><td>ERC1155Holder</td><td></td><td>7</td><td>2</td><td>9</td><td></td></tr>
    <tr><td>ERC20</td><td></td><td>122</td><td>34</td><td>156</td><td></td></tr>
    <tr><td>ERC20Burnable</td><td></td><td>13</td><td>3</td><td>16</td><td></td></tr>
    <tr><td>ERC20Capped</td><td></td><td>5</td><td>3</td><td>8</td><td></td></tr>
    <tr><td>ERC20FlashMint</td><td></td><td>12</td><td>4</td><td>16</td><td></td></tr>
    <tr><td>ERC20Pausable</td><td></td><td>12</td><td>4</td><td>16</td><td></td></tr>
    <tr><td>ERC20Permit</td><td></td><td>6</td><td>3</td><td>9</td><td></td></tr>
    <tr><td>ERC20Votes</td><td></td><td>92</td><td>30</td><td>122</td><td></td></tr>
    <tr><td>ERC20Wrapper</td><td></td><td>44</td><td>12</td><td>56</td><td></td></tr>
    <tr><td>ERC4626</td><td></td><td>71</td><td>11</td><td>82</td><td></td></tr>
    <tr><td>SafeERC20</td><td></td><td>35</td><td>12</td><td>47</td><td></td></tr>
    <tr><td>ERC721</td><td></td><td>378</td><td>71</td><td>449</td><td></td></tr>
    <tr><td>ERC721Enumerable</td><td></td><td>400</td><td>80</td><td>480</td><td></td></tr>
    <tr><td>ERC721Burnable</td><td></td><td>5</td><td>4</td><td>9</td><td></td></tr>
    <tr><td>ERC721Consecutive</td><td></td><td>34</td><td>22</td><td>56</td><td></td></tr>
    <tr><td>ERC721Pausable</td><td></td><td>9</td><td>5</td><td>14</td><td></td></tr>
    <tr><td>ERC721Royalty</td><td></td><td>16</td><td>4</td><td>20</td><td></td></tr>
    <tr><td>ERC721URIStorage</td><td></td><td>17</td><td>6</td><td>23</td><td></td></tr>
    <tr><td>ERC721Votes</td><td></td><td>25</td><td>7</td><td>32</td><td></td></tr>
    <tr><td>ERC721Wrapper</td><td></td><td>384</td><td>72</td><td>456</td><td></td></tr>
    <tr><td>ERC721Holder</td><td></td><td>1</td><td>0</td><td>1</td><td></td></tr>
    <tr><td>Address</td><td></td><td>29</td><td>14</td><td>43</td><td></td></tr>
    <tr><td>Arrays</td><td></td><td>15</td><td>0</td><td>15</td><td></td></tr>
    <tr><td>Base64</td><td></td><td>5</td><td>0</td><td>5</td><td></td></tr>
    <tr><td>Context</td><td></td><td>4</td><td>0</td><td>4</td><td></td></tr>
    <tr><td>Create2</td><td></td><td>8</td><td>2</td><td>10</td><td></td></tr>
    <tr><td>Multicall</td><td></td><td>4</td><td>2</td><td>6</td><td></td></tr>
    <tr><td>Nonces</td><td></td><td>6</td><td>1</td><td>7</td><td></td></tr>
    <tr><td>Pausable</td><td></td><td>11</td><td>5</td><td>16</td><td></td></tr>
    <tr><td>ReentrancyGuard</td><td></td><td>6</td><td>3</td><td>9</td><td></td></tr>
    <tr><td>ShortStrings</td><td></td><td>14</td><td>6</td><td>20</td><td></td></tr>
    <tr><td>StorageSlot</td><td></td><td>24</td><td>0</td><td>24</td><td></td></tr>
    <tr><td>Strings</td><td></td><td>71</td><td>1</td><td>72</td><td></td></tr>
    <tr><td>ECDSA</td><td></td><td>15</td><td>11</td><td>26</td><td></td></tr>
    <tr><td>EIP712</td><td></td><td>13</td><td>0</td><td>13</td><td></td></tr>
    <tr><td>MerkleProof</td><td></td><td>10</td><td>3</td><td>13</td><td></td></tr>
    <tr><td>MessageHashUtils</td><td></td><td>4</td><td>0</td><td>4</td><td></td></tr>
    <tr><td>ERC165</td><td></td><td>5</td><td>2</td><td>7</td><td></td></tr>
    <tr><td>ERC165Checker</td><td></td><td>40</td><td>0</td><td>40</td><td></td></tr>
    <tr><td>Math</td><td></td><td>44</td><td>1</td><td>45</td><td></td></tr>
    <tr><td>SafeCast</td><td></td><td>444</td><td>190</td><td>634</td><td></td></tr>
    <tr><td>SignedMath</td><td></td><td>12</td><td>0</td><td>12</td><td></td></tr>
    <tr><td>BitMap</td><td></td><td>10</td><td>0</td><td>10</td><td></td></tr>
    <tr><td>Checkpoints</td><td></td><td>33</td><td>3</td><td>36</td><td></td></tr>
    <tr><td>DoubleEndedQueue</td><td></td><td>9</td><td>2</td><td>11</td><td></td></tr>
    <tr><td>EnumerableMap</td><td></td><td>60</td><td>5</td><td>65</td><td></td></tr>
    <tr><td>EnumerableSet</td><td></td><td>24</td><td>0</td><td>24</td><td></td></tr>
    <tr><td>Time</td><td></td><td>7</td><td>0</td><td>7</td><td></td></tr>
    <tr><td>GovernorStorage</td><td></td><td>0</td><td>2</td><td>2</td><td></td></tr>
    <tr><td>GovernorTimelockAccess</td><td></td><td>0</td><td>2</td><td>2</td><td></td></tr>
    <tr><td>ERC1967Utils</td><td></td><td>0</td><td>3</td><td>3</td><td></td></tr>
    <tr><td>SignatureChecker</td><td></td><td>0</td><td>1</td><td>1</td><td></td></tr>
  </tbody>
</table>

