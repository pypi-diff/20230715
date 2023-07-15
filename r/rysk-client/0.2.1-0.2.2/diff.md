# Comparing `tmp/rysk_client-0.2.1.tar.gz` & `tmp/rysk_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rysk_client-0.2.1.tar", max compression
+gzip compressed data, was "rysk_client-0.2.2.tar", max compression
```

## Comparing `rysk_client-0.2.1.tar` & `rysk_client-0.2.2.tar`

### file list

```diff
@@ -1,324 +1,59 @@
--rw-r--r--   0        0        0    41561 2023-06-23 13:41:55.778268 rysk_client-0.2.1/README.md
--rw-r--r--   0        0        0      631 2023-06-23 13:41:55.782268 rysk_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/__init__.py
--rw-r--r--   0        0        0     6759 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/cli.py
--rw-r--r--   0        0        0    22900 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/client.py
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/Accounting.sol/Accounting.dbg.json
--rw-r--r--   0        0        0    32509 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/Accounting.sol/Accounting.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.dbg.json
--rw-r--r--   0        0        0    55200 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/AlphaOptionHandler.sol/AlphaOptionHandler.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0    58641 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/AlphaPortfolioValuesFeed.sol/AlphaPortfolioValuesFeed.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/Authority.sol/Authority.dbg.json
--rw-r--r--   0        0        0    14683 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/Authority.sol/Authority.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.dbg.json
--rw-r--r--   0        0        0    69533 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/BeyondPricer.sol/BeyondPricer.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.782268 rysk_client-0.2.1/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.dbg.json
--rw-r--r--   0        0        0   134569 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/LiquidityPool.sol/LiquidityPool.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/Manager.sol/Manager.dbg.json
--rw-r--r--   0        0        0    43720 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/Manager.sol/Manager.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.dbg.json
--rw-r--r--   0        0        0    30256 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/OptionCatalogue.sol/OptionCatalogue.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/OptionExchange.sol/OptionExchange.dbg.json
--rw-r--r--   0        0        0   129629 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/OptionExchange.sol/OptionExchange.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.dbg.json
--rw-r--r--   0        0        0   105395 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/OptionRegistry.sol/OptionRegistry.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/PriceFeed.sol/PriceFeed.dbg.json
--rw-r--r--   0        0        0    16525 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/PriceFeed.sol/PriceFeed.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/Protocol.sol/Protocol.dbg.json
--rw-r--r--   0        0        0     9497 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/Protocol.sol/Protocol.json
--rw-r--r--   0        0        0      105 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.dbg.json
--rw-r--r--   0        0        0    50343 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/VolatilityFeed.sol/VolatilityFeed.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.dbg.json
--rw-r--r--   0        0        0     9140 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/gelato/OpynPricerResolver.sol/OpynPricerResolver.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.dbg.json
--rw-r--r--   0        0        0     8662 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/gelato/VaultCollateralMulticall.sol/VaultCollateralMulticall.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.dbg.json
--rw-r--r--   0        0        0    89973 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/hedging/GmxHedgingReactor.sol/GmxHedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.786268 rysk_client-0.2.1/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.dbg.json
--rw-r--r--   0        0        0    59661 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/hedging/PerpHedgingReactor.sol/PerpHedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.dbg.json
--rw-r--r--   0        0        0    34523 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/hedging/UniswapV3HedgingReactor.sol/UniswapV3HedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.dbg.json
--rw-r--r--   0        0        0    91201 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/hedging/UniswapV3RangeOrderReactor.sol/UniswapV3RangeOrderReactor.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.dbg.json
--rw-r--r--   0        0        0     5293 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/AddressBookInterface.sol/AddressBookInterface.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.dbg.json
--rw-r--r--   0        0        0     5198 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/AggregatorInterface.sol/AggregatorInterface.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.dbg.json
--rw-r--r--   0        0        0     2596 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.dbg.json
--rw-r--r--   0        0        0      699 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/GammaTypes.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/IController.dbg.json
--rw-r--r--   0        0        0     7300 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/IController.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.dbg.json
--rw-r--r--   0        0        0     1774 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/IOtoken.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.dbg.json
--rw-r--r--   0        0        0     4447 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/GammaInterface.sol/IOtokenFactory.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.dbg.json
--rw-r--r--   0        0        0     5466 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAccounting.sol/IAccounting.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAddressBook.sol/IAddressBook.dbg.json
--rw-r--r--   0        0        0      500 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAddressBook.sol/IAddressBook.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.dbg.json
--rw-r--r--   0        0        0     5572 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAlphaOptionHandler.sol/IAlphaOptionHandler.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0     6033 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAlphaPortfolioValuesFeed.sol/IAlphaPortfolioValuesFeed.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.dbg.json
--rw-r--r--   0        0        0     3351 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IAuthority.sol/IAuthority.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.dbg.json
--rw-r--r--   0        0        0      657 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IChainlinkPricer.sol/IChainlinkPricer.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.dbg.json
--rw-r--r--   0        0        0    35992 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.dbg.json
--rw-r--r--   0        0        0     6762 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IGmxVaultPriceFeed.sol/IVaultPriceFeed.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.dbg.json
--rw-r--r--   0        0        0     1789 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IHedgingReactor.sol/IHedgingReactor.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.dbg.json
--rw-r--r--   0        0        0    21076 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.dbg.json
--rw-r--r--   0        0        0     1610 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IMarginCalculator.sol/IMarginCalculator.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.dbg.json
--rw-r--r--   0        0        0     8964 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IOracle.sol/IOracle.dbg.json
--rw-r--r--   0        0        0     1714 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IOracle.sol/IOracle.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0     3777 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IPortfolioValuesFeed.sol/IPortfolioValuesFeed.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.790268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.dbg.json
--rw-r--r--   0        0        0     7286 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IPositionRouter.sol/IPositionRouter.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.dbg.json
--rw-r--r--   0        0        0     2430 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IPriceFeedTimelock.sol/IPriceFeedTimelock.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IReader.sol/IReader.dbg.json
--rw-r--r--   0        0        0     1099 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IReader.sol/IReader.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IRouter.sol/IRouter.dbg.json
--rw-r--r--   0        0        0     4125 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IRouter.sol/IRouter.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.dbg.json
--rw-r--r--   0        0        0     3225 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/IWhitelist.sol/IWhitelist.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.dbg.json
--rw-r--r--   0        0        0     4001 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/I_ERC20.sol/I_ERC20.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.dbg.json
--rw-r--r--   0        0        0     4570 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/OtokenInterface.sol/OtokenInterface.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/WETH.sol/WETH.dbg.json
--rw-r--r--   0        0        0     3229 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/interfaces/WETH.sol/WETH.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.dbg.json
--rw-r--r--   0        0        0    40159 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/lens/DHVLensMK1.sol/DHVLensMK1.json
--rw-r--r--   0        0        0      956 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/lens/UserPositionLensMK1.sol/UserPositionLensMK1.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.dbg.json
--rw-r--r--   0        0        0     1163 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/AccessControl.sol/AccessControl.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.dbg.json
--rw-r--r--   0        0        0    37568 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/BlackScholes.sol/BlackScholes.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.dbg.json
--rw-r--r--   0        0        0      704 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/CombinedActions.sol/CombinedActions.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.dbg.json
--rw-r--r--   0        0        0     7217 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/CustomErrors.sol/CustomErrors.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.dbg.json
--rw-r--r--   0        0        0      700 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/EnumerableSet.sol/EnumerableSet.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.dbg.json
--rw-r--r--   0        0        0    18234 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/NormalDist.sol/NormalDist.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.dbg.json
--rw-r--r--   0        0        0     9215 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/OptionsCompute.sol/OptionsCompute.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.dbg.json
--rw-r--r--   0        0        0    33677 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/OpynInteractions.sol/OpynInteractions.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.dbg.json
--rw-r--r--   0        0        0      696 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/RyskActions.sol/RyskActions.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/SABR.sol/SABR.dbg.json
--rw-r--r--   0        0        0      682 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/SABR.sol/SABR.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.dbg.json
--rw-r--r--   0        0        0      704 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/SafeTransferLib.sol/SafeTransferLib.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/Types.sol/Types.dbg.json
--rw-r--r--   0        0        0      684 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/libraries/Types.sol/Types.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.dbg.json
--rw-r--r--   0        0        0     1207 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/ForceSend.sol/ForceSend.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.dbg.json
--rw-r--r--   0        0        0     6246 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/MockChainlinkAggregator.sol/MockChainlinkAggregator.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.dbg.json
--rw-r--r--   0        0        0     2861 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/MockChainlinkSequencerFeed.sol/MockChainlinkSequencerFeed.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.dbg.json
--rw-r--r--   0        0        0    23550 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/mocks/MockPortfolioValuesFeed.sol/MockPortfolioValuesFeed.json
--rw-r--r--   0        0        0     4355 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/otoken.json
--rw-r--r--   0        0        0      111 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.dbg.json
--rw-r--r--   0        0        0     2244 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/Migrations.sol/Migrations.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.dbg.json
--rw-r--r--   0        0        0    27786 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/AddressBook.sol/AddressBook.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.dbg.json
--rw-r--r--   0        0        0   127044 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Controller.sol/Controller.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.794268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.dbg.json
--rw-r--r--   0        0        0    89218 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/MarginCalculator.sol/MarginCalculator.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.dbg.json
--rw-r--r--   0        0        0    30610 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/MarginPool.sol/MarginPool.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.dbg.json
--rw-r--r--   0        0        0    36101 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Oracle.sol/Oracle.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.dbg.json
--rw-r--r--   0        0        0    60378 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Otoken.sol/Otoken.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.dbg.json
--rw-r--r--   0        0        0    24205 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/OtokenFactory.sol/OtokenFactory.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.dbg.json
--rw-r--r--   0        0        0      565 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/OtokenSpawner.sol/OtokenSpawner.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.dbg.json
--rw-r--r--   0        0        0    24760 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/core/Whitelist.sol/Whitelist.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.dbg.json
--rw-r--r--   0        0        0     3477 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/external/callees/PermitCallee.sol/PermitCallee.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.dbg.json
--rw-r--r--   0        0        0    14660 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/external/canonical-weth/WETH9.sol/WETH9.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.dbg.json
--rw-r--r--   0        0        0    21982 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/external/proxies/PayableProxyController.sol/PayableProxyController.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.dbg.json
--rw-r--r--   0        0        0     5307 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/AddressBookInterface.sol/AddressBookInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.dbg.json
--rw-r--r--   0        0        0     5212 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/AggregatorInterface.sol/AggregatorInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.dbg.json
--rw-r--r--   0        0        0      781 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/CTokenInterface.sol/CTokenInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.dbg.json
--rw-r--r--   0        0        0      653 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/CalleeInterface.sol/CalleeInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.dbg.json
--rw-r--r--   0        0        0     4639 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/ERC20Interface.sol/ERC20Interface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.dbg.json
--rw-r--r--   0        0        0     4342 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/MarginCalculatorInterface.sol/MarginCalculatorInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.dbg.json
--rw-r--r--   0        0        0     3944 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/MarginPoolInterface.sol/MarginPoolInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.dbg.json
--rw-r--r--   0        0        0     1017 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/OpynPricerInterface.sol/OpynPricerInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.dbg.json
--rw-r--r--   0        0        0     7103 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/OracleInterface.sol/OracleInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.dbg.json
--rw-r--r--   0        0        0     4584 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/OtokenInterface.sol/OtokenInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.dbg.json
--rw-r--r--   0        0        0     2475 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/WETH9Interface.sol/WETH9Interface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.dbg.json
--rw-r--r--   0        0        0     1266 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/WSTETHInterface.sol/WSTETHInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.dbg.json
--rw-r--r--   0        0        0     7545 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/WhitelistInterface.sol/WhitelistInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.dbg.json
--rw-r--r--   0        0        0     1789 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/YearnVaultInterface.sol/YearnVaultInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.dbg.json
--rw-r--r--   0        0        0     3503 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/interfaces/ZeroXExchangeInterface.sol/ZeroXExchangeInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.dbg.json
--rw-r--r--   0        0        0      657 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/Actions.sol/Actions.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.dbg.json
--rw-r--r--   0        0        0      675 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/FixedPointInt256.sol/FixedPointInt256.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.dbg.json
--rw-r--r--   0        0        0    11131 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/MarginVault.sol/MarginVault.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.dbg.json
--rw-r--r--   0        0        0      673 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/libs/SignedConverter.sol/SignedConverter.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.dbg.json
--rw-r--r--   0        0        0    94183 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewCalculator.sol/NewMarginCalculator.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.dbg.json
--rw-r--r--   0        0        0   129863 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewController.sol/NewController.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.dbg.json
--rw-r--r--   0        0        0     4096 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewMarginCalculatorInterface.sol/MarginCalculatorInterface.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.dbg.json
--rw-r--r--   0        0        0    31173 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/new/NewWhitelist.sol/NewWhitelist.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.dbg.json
--rw-r--r--   0        0        0      701 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/BokkyPooBahsDateTimeLibrary.sol/BokkyPooBahsDateTimeLibrary.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.dbg.json
--rw-r--r--   0        0        0     1713 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/Spawn.sol/Spawn.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.dbg.json
--rw-r--r--   0        0        0      664 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Address.sol/Address.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Context.sol/Context.dbg.json
--rw-r--r--   0        0        0      250 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Context.sol/Context.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.dbg.json
--rw-r--r--   0        0        0      664 2023-06-23 13:41:55.798268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Create2.sol/Create2.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.dbg.json
--rw-r--r--   0        0        0     4014 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/IERC20.sol/IERC20.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.dbg.json
--rw-r--r--   0        0        0     1345 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Ownable.sol/Ownable.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
--rw-r--r--   0        0        0      266 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/ReentrancyGuard.sol/ReentrancyGuard.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.dbg.json
--rw-r--r--   0        0        0      668 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/SafeERC20.sol/SafeERC20.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.dbg.json
--rw-r--r--   0        0        0      666 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/SafeMath.sol/SafeMath.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.dbg.json
--rw-r--r--   0        0        0      678 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/SignedSafeMath.sol/SignedSafeMath.json
--rw-r--r--   0        0        0      117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.dbg.json
--rw-r--r--   0        0        0      664 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/Strings.sol/Strings.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.dbg.json
--rw-r--r--   0        0        0    16052 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ERC20Upgradeable.sol/ERC20Upgradeable.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/GSN/ContextUpgradeable.sol/ContextUpgradeable.dbg.json
--rw-r--r--   0        0        0      291 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/GSN/ContextUpgradeable.sol/ContextUpgradeable.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.dbg.json
--rw-r--r--   0        0        0     4051 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/IERC20Upgradeable.sol/IERC20Upgradeable.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.dbg.json
--rw-r--r--   0        0        0      587 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Initializable.sol/Initializable.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.dbg.json
--rw-r--r--   0        0        0     4294 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnableUpgradeSafe.sol/OwnableUpgradeSafe.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.dbg.json
--rw-r--r--   0        0        0     7531 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/OwnedUpgradeabilityProxy.sol/OwnedUpgradeabilityProxy.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.dbg.json
--rw-r--r--   0        0        0      595 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/Proxy.sol/Proxy.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.dbg.json
--rw-r--r--   0        0        0      613 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/ReentrancyGuardUpgradeSafe.sol/ReentrancyGuardUpgradeSafe.json
--rw-r--r--   0        0        0      120 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.dbg.json
--rw-r--r--   0        0        0     2001 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/UpgradeabilityProxy.sol/UpgradeabilityProxy.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.dbg.json
--rw-r--r--   0        0        0      546 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/cryptography/ECDSAUpgradeable.sol/ECDSAUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/EIP712Upgradeable.sol/EIP712Upgradeable.dbg.json
--rw-r--r--   0        0        0      298 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/EIP712Upgradeable.sol/EIP712Upgradeable.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.dbg.json
--rw-r--r--   0        0        0     7379 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/ERC20PermitUpgradeable.sol/ERC20PermitUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.dbg.json
--rw-r--r--   0        0        0     1870 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/erc20-permit/IERC20PermitUpgradeable.sol/IERC20PermitUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.dbg.json
--rw-r--r--   0        0        0      544 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/math/SafeMathUpgradeable.sol/SafeMathUpgradeable.json
--rw-r--r--   0        0        0      123 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.dbg.json
--rw-r--r--   0        0        0      545 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/packages/oz/upgradeability/utils/CountersUpgradeable.sol/CountersUpgradeable.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.dbg.json
--rw-r--r--   0        0        0    12510 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/ChainlinkPricer.sol/ChainLinkPricer.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.dbg.json
--rw-r--r--   0        0        0    10253 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/CompoundPricer.sol/CompoundPricer.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.dbg.json
--rw-r--r--   0        0        0     9115 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/WstethPricer.sol/WstethPricer.json
--rw-r--r--   0        0        0      114 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.dbg.json
--rw-r--r--   0        0        0    10339 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/packages/opyn/pricers/YearnPricer.sol/YearnPricer.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/tokens/ERC20.sol/ERC20.dbg.json
--rw-r--r--   0        0        0     6254 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/tokens/ERC20.sol/ERC20.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.dbg.json
--rw-r--r--   0        0        0    20725 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/tokens/MintableERC20.sol/MintableERC20.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/tokens/WETH.sol/WETH.dbg.json
--rw-r--r--   0        0        0    14042 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/tokens/WETH.sol/WETH.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.dbg.json
--rw-r--r--   0        0        0      698 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholes.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.dbg.json
--rw-r--r--   0        0        0    26324 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/BlackScholesTest.sol/BlackScholesTest.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.dbg.json
--rw-r--r--   0        0        0      696 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/BlackScholesTest.sol/NormalDist.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.dbg.json
--rw-r--r--   0        0        0    14566 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/LiquidityPoolAdjustCollateralTest.sol/LiquidityPoolAdjustCollateralTest.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/OracleMock.sol/OracleMock.dbg.json
--rw-r--r--   0        0        0     7244 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/OracleMock.sol/OracleMock.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.dbg.json
--rw-r--r--   0        0        0     8117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/PerpHedgingTest.sol/PerpHedgingTest.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.dbg.json
--rw-r--r--   0        0        0    39837 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/RealTokenMock.sol/RealTokenMock.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.dbg.json
--rw-r--r--   0        0        0      668 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/ReentrancyGuard.sol/ReentrancyGuard.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.dbg.json
--rw-r--r--   0        0        0    17149 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/UniswapConversionsTest.sol/UniswapConversionsTest.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.dbg.json
--rw-r--r--   0        0        0     8046 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/UniswapV3HedgingTest.sol/UniswapV3HedgingTest.json
--rw-r--r--   0        0        0      108 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/Volatility.sol/Volatility.dbg.json
--rw-r--r--   0        0        0     5933 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/utils/Volatility.sol/Volatility.json
--rw-r--r--   0        0        0      111 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.dbg.json
--rw-r--r--   0        0        0      695 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/FullMath.sol/FullMath.json
--rw-r--r--   0        0        0      111 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.dbg.json
--rw-r--r--   0        0        0      711 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/LiquidityAmounts.sol/LiquidityAmounts.json
--rw-r--r--   0        0        0      111 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.dbg.json
--rw-r--r--   0        0        0      701 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/PoolAddress.sol/PoolAddress.json
--rw-r--r--   0        0        0      111 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.dbg.json
--rw-r--r--   0        0        0      845 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/contracts/vendor/uniswap/TickMath.sol/TickMath.json
--rw-r--r--   0        0        0      499 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/action_type.py
--rw-r--r--   0        0        0      860 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/collateral.py
--rw-r--r--   0        0        0     5634 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/constants.py
--rw-r--r--   0        0        0      212 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/crypto.py
--rw-r--r--   0        0        0      185 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/exceptions.py
--rw-r--r--   0        0        0     8117 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/operation_factory.py
--rw-r--r--   0        0        0      507 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/order.py
--rw-r--r--   0        0        0      182 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/order_side.py
--rw-r--r--   0        0        0     4538 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/pnl_calculator.py
--rw-r--r--   0        0        0      592 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/position.py
--rw-r--r--   0        0        0     1114 2023-06-23 13:41:55.802268 rysk_client-0.2.1/rysk_client/src/position_manager.py
--rw-r--r--   0        0        0      193 2023-06-23 13:41:55.806268 rysk_client-0.2.1/rysk_client/src/position_side.py
--rw-r--r--   0        0        0     7530 2023-06-23 13:41:55.806268 rysk_client-0.2.1/rysk_client/src/rysk_option_market.py
--rw-r--r--   0        0        0     3106 2023-06-23 13:41:55.806268 rysk_client-0.2.1/rysk_client/src/subgraph.py
--rw-r--r--   0        0        0     2027 2023-06-23 13:41:55.806268 rysk_client-0.2.1/rysk_client/src/utils.py
--rw-r--r--   0        0        0    10844 2023-06-23 13:41:55.806268 rysk_client-0.2.1/rysk_client/web3_client.py
--rw-r--r--   0        0        0    42155 1970-01-01 00:00:00.000000 rysk_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    45006 2023-07-15 13:02:33.149161 rysk_client-0.2.2/README.md
+-rw-r--r--   0        0        0      709 2023-07-15 13:02:33.153161 rysk_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/__init__.py
+-rw-r--r--   0        0        0     9030 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/cli.py
+-rw-r--r--   0        0        0    25070 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/client.py
+-rw-r--r--   0        0        0      974 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
+-rw-r--r--   0        0        0    35992 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
+-rw-r--r--   0        0        0    13187 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
+-rw-r--r--   0        0        0      527 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
+-rw-r--r--   0        0        0      971 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
+-rw-r--r--   0        0        0    35311 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
+-rw-r--r--   0        0        0     6580 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
+-rw-r--r--   0        0        0      601 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
+-rw-r--r--   0        0        0      968 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/__init__.py
+-rw-r--r--   0        0        0    15813 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
+-rw-r--r--   0        0        0     8845 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/contract.py
+-rw-r--r--   0        0        0      509 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
+-rw-r--r--   0        0        0    38053 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
+-rw-r--r--   0        0        0    11285 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
+-rw-r--r--   0        0        0      533 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
+-rw-r--r--   0        0        0    42143 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
+-rw-r--r--   0        0        0    13308 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
+-rw-r--r--   0        0        0      533 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
+-rw-r--r--   0        0        0      981 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
+-rw-r--r--   0        0        0    38232 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
+-rw-r--r--   0        0        0    10787 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
+-rw-r--r--   0        0        0      547 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/__init__.py
+-rw-r--r--   0        0        0    11137 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
+-rw-r--r--   0        0        0     6104 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/contract.py
+-rw-r--r--   0        0        0      580 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
+-rw-r--r--   0        0        0      979 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
+-rw-r--r--   0        0        0     2515 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
+-rw-r--r--   0        0        0     4220 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
+-rw-r--r--   0        0        0      541 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/__init__.py
+-rw-r--r--   0        0        0    15880 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/build/weth.json
+-rw-r--r--   0        0        0     6490 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/contract.py
+-rw-r--r--   0        0        0      580 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/contract.yaml
+-rw-r--r--   0        0        0      488 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/packages.json
+-rw-r--r--   0        0        0      690 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/action_type.py
+-rw-r--r--   0        0        0      856 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/collateral.py
+-rw-r--r--   0        0        0     4875 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/constants.py
+-rw-r--r--   0        0        0      212 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/crypto.py
+-rw-r--r--   0        0        0      185 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/exceptions.py
+-rw-r--r--   0        0        0     8518 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/operation_factory.py
+-rw-r--r--   0        0        0      507 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/order.py
+-rw-r--r--   0        0        0      182 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/order_side.py
+-rw-r--r--   0        0        0     4538 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/pnl_calculator.py
+-rw-r--r--   0        0        0      592 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/position.py
+-rw-r--r--   0        0        0     1114 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/position_manager.py
+-rw-r--r--   0        0        0      193 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/position_side.py
+-rw-r--r--   0        0        0     7830 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/rysk_option_market.py
+-rw-r--r--   0        0        0     3282 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/subgraph.py
+-rw-r--r--   0        0        0     2341 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/utils.py
+-rw-r--r--   0        0        0    15436 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/web3_client.py
+-rw-r--r--   0        0        0    45592 1970-01-01 00:00:00.000000 rysk_client-0.2.2/PKG-INFO
```

### Comparing `rysk_client-0.2.1/README.md` & `rysk_client-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: rysk-client
+Version: 0.2.2
+Summary: 
+Author: 8baller
+Author-email: 8ball030@gmail.com
+Requires-Python: >=3.8,<=3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ccxt (>=1.72.82)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Requires-Dist: web3 (>=5,<6)
+Requires-Dist: websocket-client (>=0.32.0,<1)
+Description-Content-Type: text/markdown
+
 # Rysk Client
 
 ## Installation
 
 The application is availale on pypi and can be installed as so;
 
     ```bash
@@ -182,14 +200,18 @@
     │ ETH-30JUN… │ short │ 0          │ 0x9b8a20… │ 0.0   │ 0.0        │ 21249.08… │
     │ ETH-30JUN… │ short │ 105.35629… │ 0x9b8a20… │ -2.0  │ 210.712583 │ 0         │
     │ ETH-30JUN… │ short │ 118.16245… │ 0x9b8a20… │ -14.0 │ 1654.2744… │ 0         │
     │ ETH-30JUN… │ short │ 106.420235 │ 0x9b8a20… │ -1.0  │ 106.420235 │ 0         │
     └────────────┴───────┴────────────┴───────────┴───────┴────────────┴───────────┘
 
 
+## Expired positions
+
+We can use the `--expired` flag in order to filter for the expired positions
+
 
 ```python
 ! export ETH_ADDRESS=0x9B8a204636a7aa9c33053d9C3A828720d32212e8 && \
   export ETH_PRIVATE_KEY=0x75cc9212e9e1243b9a3e5db5012f39469254088e33363324ad94dd0b212d7efa && \
     rysk positions list --expired
 ```
 
@@ -222,19 +244,54 @@
     │ ETH-16JU… │ short │ 21.762156… │ 0x9b8a20… │ -20.0  │ 435.24313… │ 0         │
     │ ETH-26MA… │ short │ 50.9876923 │ 0x9b8a20… │ -10.0  │ 509.876923 │ 0         │
     │ ETH-02JU… │ short │ 31.792668  │ 0x9b8a20… │ -1.0   │ 31.792668  │ 0         │
     │ ETH-26MA… │ short │ 47.281672… │ 0x9b8a20… │ -40.0  │ 1891.2668… │ 0         │
     └───────────┴───────┴────────────┴───────────┴────────┴────────────┴───────────┘
 
 
+## Settling Positions
+We are able to settle the positions based on the vault id
+
 
 ```python
 
+! export ETH_ADDRESS=0x9B8a204636a7aa9c33053d9C3A828720d32212e8 && \
+  export ETH_PRIVATE_KEY=0x75cc9212e9e1243b9a3e5db5012f39469254088e33363324ad94dd0b212d7efa && \
+  rysk positions settle -v 15
 ```
 
+    [2;36m[06/23/23 01:02:47][0m[2;36m [0m[34mINFO    [0m Settling vault [1;36m15[0m for                    ]8;id=770874;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/cli.py\[2mcli.py[0m]8;;\[2m:[0m]8;id=837991;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/cli.py#148\[2m148[0m]8;;\
+    [2;36m                    [0m         [1;36m0x9B8a204636a7aa9c33053d9C3A828720d32212[0m [2m          [0m
+    [2;36m                    [0m         [1;36me8[0m                                       [2m          [0m
+    [2;36m                   [0m[2;36m [0m[34mINFO    [0m Rysk client initialized and connected  ]8;id=936728;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/client.py\[2mclient.py[0m]8;;\[2m:[0m]8;id=522814;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/client.py#99\[2m99[0m]8;;\
+    [2;36m                    [0m         to the blockchain at RPC connection    [2m            [0m
+    [2;36m                    [0m         [4;94mhttps://arbitrum-goerli.rpc.thirdweb.c[0m [2m            [0m
+    [2;36m                    [0m         [4;94mom[0m                                     [2m            [0m
+    Traceback (most recent call last):
+      File "/home/tom/.pyenv/versions/3.10.4/bin/rysk", line 8, in <module>
+        sys.exit(cli())
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1126, in __call__
+        return self.main(*args, **kwargs)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rich_click/rich_group.py", line 21, in main
+        rv = super().main(*args, standalone_mode=False, **kwargs)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1051, in main
+        rv = self.invoke(ctx)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1657, in invoke
+        return _process_result(sub_ctx.command.invoke(sub_ctx))
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1657, in invoke
+        return _process_result(sub_ctx.command.invoke(sub_ctx))
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1393, in invoke
+        return ctx.invoke(self.callback, **ctx.params)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 752, in invoke
+        return __callback(*args, **kwargs)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/cli.py", line 158, in settle
+        raise ValueError(
+    ValueError: Vault 15 has already been settled for 0x9B8a204636a7aa9c33053d9C3A828720d32212e8
+
+
 ## Creating a Client 
 
 Clients can be created from the rysk client module.
 
 
 ```python
 from rysk_client.client import RyskClient
@@ -571,7 +628,24 @@
     [1mAll done! ✨ 🍰 ✨[0m
     [34m19 files [0mleft unchanged.
     poetry run adev lint -v -p tests
     [2;36m[14:13:44][0m[2;36m [0m[34mINFO    [0m Linting Open Autonomy Packages                     ]8;id=281004;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py\[2mcli.py[0m]8;;\[2m:[0m]8;id=265993;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py#47\[2m47[0m]8;;\
     [2KLinting... [38;2;114;156;31m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [35m100%[0m [33m0:00:03[0m
     [?25h[2;36m[14:13:48][0m[2;36m [0m[34mINFO    [0m Linting completed successfully!                    ]8;id=864081;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py\[2mcli.py[0m]8;;\[2m:[0m]8;id=992553;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py#66\[2m66[0m]8;;\
 
+
+
+```python
+
+```
+
+# Releasing
+Git ops is used to enable automated releases via pypi.
+
+```bash
+export NEW_VERSION=0.2.0
+git checkout -b v$NEW_VERSION
+bumpversion  rysk_client/ --new-version $NEW_VERSION
+git push && git push --tag
+
+```
+
```

### Comparing `rysk_client-0.2.1/rysk_client/client.py` & `rysk_client-0.2.2/rysk_client/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 """
 Simple client for the rysk contracts implemented in python.
 """
-import logging
+import time
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
-from rich import print_json
+import web3
 
-from rysk_client.src.action_type import ActionType
 from rysk_client.src.collateral import Collateral
-from rysk_client.src.constants import NULL_ADDRESS, NULL_DATA, RPC_URL
+from rysk_client.src.constants import ARBITRUM_GOERLI, Chain
 from rysk_client.src.crypto import EthCrypto
+from rysk_client.src.operation_factory import buy, sell
 from rysk_client.src.order_side import OrderSide
 from rysk_client.src.pnl_calculator import PnlCalculator, Trade
 from rysk_client.src.position_side import PositionSide
 from rysk_client.src.rysk_option_market import OptionChain, RyskOptionMarket
 from rysk_client.src.subgraph import SubgraphClient
 from rysk_client.src.utils import get_contract, get_logger
-from rysk_client.web3_client import Web3Client
+from rysk_client.web3_client import Web3Client, print_operate_tuple
 
 PRICE_DEVISOR = 1_000_000_000_000_000_000
 EXPOSURE_DEVISOR = 1_000_000_000_000_000_000
 
-ALLOWED_SLIPPAGE = 0.1
+ALLOWED_SLIPPAGE = 0.15
+
+NULL_SERIES = (
+    0,
+    0,
+    False,
+    "0x0000000000000000000000000000000000000000",
+    "0x0000000000000000000000000000000000000000",
+    "0x0000000000000000000000000000000000000000",
+)
 
 
 class ApprovalException(Exception):
     """
     Exception raised when the approval fails.
     """
 
@@ -72,37 +81,81 @@
     """
     Client for the rysk contracts.
     """
 
     _markets: List[RyskOptionMarket]
     _tickers: List[Dict[str, Any]]
     _otokens: Dict[str, Dict[str, Any]]
+    web3_client: Web3Client
 
     def __init__(
         self,
         address: Optional[str] = None,
         private_key: Optional[str] = None,
         logger=None,
-        rpc_url: str = RPC_URL,
+        chain: Chain = ARBITRUM_GOERLI,
+        verbose: bool = True,
     ):
         self._markets: List[RyskOptionMarket] = []
         self._tickers = []
         self._otokens = {}
         self._option_chain: OptionChain
         self._crypto = EthCrypto(address, private_key)
         self._logger = logger or get_logger()
         self.web3_client = Web3Client(
             self._logger,
             self._crypto,
-            rpc_url=rpc_url,
+            chain=chain,
+            verbose=verbose,
         )
         self.subgraph_client = SubgraphClient()
         self._logger.info(
             f"Rysk client initialized and connected to the blockchain at {self.web3_client.web3.provider}"
         )
+        self._verbose = verbose
+
+    def _sign_and_sumbit(self, txn, retries=3, backoff=2):
+        """
+        Sign and submit transaction.
+
+        retries: number of retries
+        backoff: backoff in seconds
+
+        """
+        try:
+            txn["nonce"] = self.web3_client.web3.eth.get_transaction_count(
+                self._crypto.address
+            )
+            signed_txn = self.web3_client.web3.eth.account.sign_transaction(
+                txn, private_key=self._crypto.private_key
+            )
+            tx_hash = self.web3_client.web3.eth.send_raw_transaction(
+                signed_txn.rawTransaction
+            )
+            self._logger.debug(f"Transaction hash: {tx_hash.hex()}")
+            receipt = self.web3_client.web3.eth.wait_for_transaction_receipt(
+                tx_hash, 180
+            )
+            # we need to check the receipt to see if the transaction was successful
+            if receipt["status"] == 0:
+                self._logger.error(f"Transaction failed: {receipt}")
+                raise ValueError("Transaction Failed!")
+            self._logger.debug(f"Transaction successful: {receipt}")
+            return tx_hash.hex()
+
+        except ValueError as error:
+            if retries > 0:
+                self._logger.warning(
+                    f"Error {error} while submitting transaction. Retrying..."
+                )
+                time.sleep(backoff)
+                return self._sign_and_sumbit(
+                    txn, retries=retries - 1, backoff=backoff * 2
+                )
+            raise error
 
     def fetch_markets(self) -> List[Dict[str, Any]]:
         """
         Fetchs the markets from the subgraph.
         """
 
         raw_data = self.web3_client.get_option_chain()
@@ -111,15 +164,15 @@
             RyskOptionMarket.from_option_drill(*data)
             for data in self._option_chain.active_markets
         ]
         return [market.to_json() for market in self._markets]  # type: ignore
 
     def to_checksum_address(self, address):
         """Convert an address to a checksum address."""
-        return self.web3_client.web3.to_checksum_address(address)
+        return self.web3_client.web3.toChecksumAddress(address)
 
     def fetch_tickers(
         self, market: Optional[str] = None, is_active: Optional[bool] = True
     ) -> List[Dict[str, Any]]:
         """
         Fetchs the ticker from the beyond pricer smart contract.
         """
@@ -150,15 +203,14 @@
         """
 
         if self._crypto.address is None:
             raise ValueError("No account address was provided.")
 
         longs = self.subgraph_client.query_longs(address=self._crypto.address)
         shorts = self.subgraph_client.query_shorts(address=self._crypto.address)
-        # use the lens
 
         parsed_short = [self._parse_position(pos, PositionSide.SHORT) for pos in shorts]
         parsed_longs = [self._parse_position(pos, PositionSide.LONG) for pos in longs]
 
         if expired:
             positions = filter(
                 lambda x: x["datetime"] <= datetime.now(),
@@ -236,178 +288,158 @@
             raise ValueError("Invalid order side")
 
         if side == OrderSide.BUY.value:
             transaction = self.buy_option(symbol, amount)
         else:
             transaction = self.sell_option(symbol, amount)
         # we can now submit it to the chain;
-        transaction["nonce"] = self.web3_client.web3.eth.get_transaction_count(
-            self._crypto.address
-        )
-        submitted = self.web3_client.sign_and_sumbit(
-            transaction, self._crypto.private_key
-        )
-        if submitted:
-            self._logger.info(f"Order for {amount} {symbol} Successfully created!")
-            self._logger.info(f"Transaction hash: {submitted}")
-        else:
-            self._logger.error(f"Order for {amount} {symbol} failed to create!")
-            raise ValueError("Order failed to create.")
+        # we can also confirm the otoken balance
+        market = self.get_market(symbol)
+        otoken_address = self.web3_client.get_otoken(market.to_series())
+
+        old_balance = self.web3_client.get_otoken_balance(otoken_address)
+
+        self._logger.info(f"Otken balance: {old_balance}")
+        block_number = self.web3_client.web3.eth.block_number
+        submitted = self._sign_and_sumbit(transaction)
+        # block until the transaction is mined
+        wait = 10
+        while self.web3_client.web3.eth.block_number <= block_number:
+            time.sleep(1)
+            wait -= 1
+            if wait == 0:
+                raise TimeoutError("Transaction was not mined in time.")
+
+        self._logger.info(f"Submitted transaction with hash: {submitted}")
+        new_balance = self.web3_client.get_otoken_balance(otoken_address)
+        self._logger.info(f"Otken balance: {new_balance}")
+        if new_balance == old_balance and side == OrderSide.BUY.value:
+            self._logger.error(
+                f"Transaction failed to execute. Balance is still {new_balance}"
+            )
+
         return {
             "id": submitted,
             "symbol": symbol,
             "datetime": datetime.now(),
         }
 
+    def get_market(self, symbol: str) -> RyskOptionMarket:
+        """
+        Returns the market information.
+        """
+        if not self._markets:
+            self.fetch_markets()
+
+        for market in self._markets:
+            if market.name == symbol:
+                return market
+        raise ValueError(f"Could not find market {symbol}.")
+
     def buy_option(  # noqa: R0914
         self,
         market: str,
         amount: float,
-        collateral_asset: str = "usdc",
+        collateral_asset: str = "USDC",
         leverage: float = 1,
     ):
         """
         Create a buy option order.
         """
+        # now we can try to buy the option
+        if not self._markets:
+            self._logger.info("Fetching Tickers.")
+            self.fetch_tickers()  # type: ignore
+
+        self._logger.info(f"Fetching acceptable premium for {market}")
+        rysk_option_market = self.get_market(market)
+        rysk_option_market.collateral = Collateral.from_symbol(collateral_asset)
         self._logger.info(
             f"Buying {amount} of {market} with {collateral_asset} collateral @ {leverage}x leverage."
         )
         # we first check the approval amount of the collateral asset
         if not Collateral.is_supported(collateral_asset):
             raise ValueError(
                 f"Collateral asset {collateral_asset} is not supported by the protocol."
             )
-        collateral_contract = get_contract(collateral_asset, self.web3_client.web3)
+        collateral_asset_name = f"{rysk_option_market.collateral.name.lower()}"
+        collateral_contract = get_contract(
+            collateral_asset_name, self.web3_client.web3, self.web3_client.chain
+        )
         collateral_approved = self.web3_client.is_approved(
             collateral_contract,
             self.web3_client.option_exchange.address,
             str(self._crypto.address),
             int(amount * 1e18),
         )
+        self._logger.info(f"Collateral approved: {collateral_approved}.")
 
         if not collateral_approved:
             self._logger.info(
                 f"Approving {collateral_asset} collateral for {self.web3_client.option_exchange.address}"
             )
 
             txn = self.web3_client.create_approval(
                 collateral_contract,
                 self.web3_client.option_exchange.address,
                 str(self._crypto.address),
                 collateral_approved + int(amount * 1e18),
             )
             # we submit and sign the transaction
-            result = self.web3_client.sign_and_sumbit(txn, self._crypto.private_key)  # type: ignore
-            if result is not None:
-                self._logger.info(f"Transaction successful with hash: {result}")
-            else:
-                self._logger.error(f"Transaction failed: {result}")
+            result = self._sign_and_sumbit(txn)
+            self._logger.info(f"Transaction successful with hash: {result}")
 
-        # now we can try to buy the option
-        if not self._markets:
-            self._logger.info("Fetching Tickers.")
-            self.fetch_tickers()  # type: ignore
+        otoken_address = self.web3_client.get_otoken(rysk_option_market.to_series())
+        balance = self.web3_client.get_otoken_balance(otoken_address)
+        self._logger.info(f"Balance of {otoken_address}: {balance}")
 
-        self._logger.info(f"Fetching acceptable premium for {market}")
-        rysk_option_market: RyskOptionMarket = [f for f in self._markets if f.name == market][0]  # type: ignore
-        _amount = amount * 1000000000000000000
+        self._logger.info(
+            f"Fetching market data for {market}. Otoken address: {otoken_address}"
+        )
+        _amount = amount * 1_000_000_000_000_000_000
         acceptable_premium = self.web3_client.get_options_prices(  # type: ignore
             rysk_option_market.to_series(),
             rysk_option_market.dhv,
             side=OrderSide.BUY.value,
             amount=_amount,
         )  # pylint: disable=E1120
 
         # we format 2 decimal places
-        self._logger.info(f"Acceptable premium: ${acceptable_premium:.2f}")
+        self._logger.info(f"Acceptable premium: ${acceptable_premium / 1e6:.2f}")
 
-        series = rysk_option_market.to_series()  # type: ignore
+        # we check if we need to issue the option
+        issuance_required = self.is_issuance_required(otoken_address)
 
-        vault_id = 20
-        user_vaults = self.web3_client.fetch_user_vaults(
-            self._crypto.address
-        )  # pylint: disable=E1120
+        operate_tuple = buy(
+            int(acceptable_premium),
+            owner_address=self._crypto.address,  # pylint: disable=E1120
+            amount=int(_amount),
+            option_market=rysk_option_market,
+            issuance_required=issuance_required,
+        )
 
-        if not user_vaults:
-            self._logger.info("No vaults found. Creating one.")
-            raise NotImplementedError("No vaults found. Creating one.")
-        # do we need to use an alternative aorder of operations?
+        if self._verbose:
+            print_operate_tuple([operate_tuple])
 
-        operate_tuple = [
-            {
-                "operation": 0,
-                "operationQueue": [
-                    {
-                        "actionType": ActionType.DEPOSIT_COLLATERAL.value,
-                        "owner": self._crypto.address,
-                        "secondAddress": self.web3_client.option_exchange.address,
-                        "asset": Collateral.from_symbol("weth").value,
-                        "vaultId": vault_id,
-                        "amount": 0,
-                        "optionSeries": {
-                            "expiration": 1,
-                            "strike": 1,
-                            "isPut": bool(series["isPut"]),
-                            "underlying": NULL_ADDRESS,
-                            "strikeAsset": NULL_ADDRESS,
-                            "collateral": NULL_ADDRESS,
-                        },
-                        "indexOrAcceptablePremium": 0,
-                        "data": "0x0000000000000000000000000000000000000000",
-                    },
-                    {
-                        "actionType": ActionType.MINT_SHORT_OPTION.value,
-                        "owner": NULL_ADDRESS,
-                        "secondAddress": str(self._crypto.address),
-                        "asset": NULL_ADDRESS,
-                        "vaultId": 0,
-                        "amount": int(_amount),
-                        "optionSeries": {
-                            "expiration": 1,
-                            "strike": 1,
-                            "isPut": True,
-                            "underlying": NULL_ADDRESS,
-                            "strikeAsset": NULL_ADDRESS,
-                            "collateral": NULL_ADDRESS,
-                        },
-                        "indexOrAcceptablePremium": 0,
-                        "data": "0x0000000000000000000000000000000000000000",
-                    },
-                ],
-            },
-            {
-                "operation": 1,
-                "operationQueue": [
-                    {
-                        "actionType": ActionType.BURN_SHORT_OPTION.value,
-                        "owner": NULL_ADDRESS,
-                        "secondAddress": self._crypto.address,
-                        "asset": NULL_ADDRESS,
-                        "vaultId": 0,
-                        "amount": int(_amount),
-                        "optionSeries": {
-                            "expiration": int(series["expiration"]),
-                            "strike": int(series["strike"]),
-                            "isPut": True,
-                            "underlying": Collateral.from_symbol("weth").value,
-                            "strikeAsset": Collateral.from_symbol("usdc").value,
-                            "collateral": Collateral.from_symbol("weth").value,
-                        },
-                        "indexOrAcceptablePremium": int(_amount),
-                        "data": NULL_DATA,
-                    },
-                ],
-            },
-        ]
+        try:
+            txn = self.web3_client.option_exchange.functions.operate(
+                [operate_tuple]
+            ).build_transaction({"from": self._crypto.address})
+        except web3.exceptions.ContractCustomError as error:  # pylint: disable=E1101
+            self._logger.error("Transaction failed due to incorrect parameters.")
+            raise ValueError(error) from error
 
-        # buy tx
-        self._logger.info(f"Passing:\n{operate_tuple}")
+        return txn
 
-        func = self.web3_client.option_exchange.functions.operate(operate_tuple)  #
-        return func
+    def is_issuance_required(self, otoken_address: str) -> bool:
+        """
+        Returns True if an issuance is required.
+        """
+        result = self.web3_client.get_series_info(otoken_address)
+        return result == NULL_SERIES
 
     def sell_option(  # noqa
         self,
         market: str,
         amount: float,
         collateral_asset: str = "weth",
         leverage: float = 1,
@@ -420,19 +452,15 @@
         )
 
         if not self._markets:
             self._logger.info("Fetching Tickers.")
             self.fetch_tickers()
         _amount = amount * 1e18
 
-        rysk_option_market: RyskOptionMarket = [
-            f for f in self._markets if f.name == market
-        ][
-            0
-        ]  # type: ignore
+        rysk_option_market = self.get_market(market)
 
         acceptable_premium = self.web3_client.get_options_prices(
             rysk_option_market.to_series(),
             dhv_exposure=rysk_option_market.dhv,
             amount=_amount,
             side=OrderSide.SELL.value,
             collateral=collateral_asset,
@@ -440,20 +468,22 @@
 
         self._logger.info(f"Acceptable premium: ${acceptable_premium:.2f}")
 
         user_vaults = self.web3_client.fetch_user_vaults(self._crypto.address)
         otoken_id = self.web3_client.get_otoken(rysk_option_market.to_series())
         self._logger.info(f"Option Otoken id is {otoken_id}")
 
+        issue_new_vault = False
         if otoken_id not in set(i[1] for i in user_vaults):
             new_vault_id = len(user_vaults) + 1
             self._logger.info(
                 f"Necessary to create a vault for the user. New vault id is {new_vault_id}"
             )
             vault_id = new_vault_id
+            issue_new_vault = True
 
         else:
             # we need to use the vault
             vault_id = [f[1] for f in user_vaults].index(otoken_id) + 1
             self._logger.info(f"Using existing vault id user_vaults {vault_id}")
 
         if rysk_option_market.is_put:
@@ -464,15 +494,15 @@
                 * (1 + ALLOWED_SLIPPAGE)
                 * 1e18
             )
             contract = self.web3_client.usdc
         else:
             collateral_asset = Collateral.WETH
             amount_to_approve = int(_amount * (1 + ALLOWED_SLIPPAGE))
-            contract = self.web3_client.weth
+            contract = self.web3_client.settlement_weth
 
         # we check the approval of the amount
         self._logger.info(
             f"Checking approval of {amount_to_approve / 1e18} of {collateral_asset}"
         )
         allowance = contract.functions.allowance(
             self._crypto.address,
@@ -485,111 +515,50 @@
                 contract=contract,
                 spender=self.web3_client.option_exchange.address,
                 owner=self._crypto.address,
                 amount=amount_to_approve,
             )
 
             self._logger.debug(f"Approve tx is {approve_tx}")
-            tx_hash = self.web3_client.sign_and_sumbit(
-                approve_tx, self._crypto.private_key
-            )
+            tx_hash = self._sign_and_sumbit(approve_tx)
             self._logger.info(f"Tx hash is {tx_hash}")
-            if not tx_hash:
-                raise ApprovalException("Approval failed.")
-        # we need to create a vault
 
-        underlying = Collateral.WETH.value
-        strike_asset = Collateral.USDC.value
-
-        operate_tuple = [
-            {
-                "operation": 0,
-                "operationQueue": [
-                    {
-                        "actionType": ActionType.DEPOSIT_COLLATERAL.value,
-                        "owner": self.to_checksum_address(self._crypto.address),
-                        "secondAddress": self.to_checksum_address(
-                            self.web3_client.option_exchange.address
-                        ),
-                        "asset": underlying,
-                        "vaultId": vault_id,
-                        "amount": int(_amount),
-                        "optionSeries": {
-                            "expiration": 1,
-                            "strike": int(rysk_option_market.strike),
-                            "isPut": True,
-                            "underlying": NULL_ADDRESS,
-                            "strikeAsset": NULL_ADDRESS,
-                            "collateral": NULL_ADDRESS,
-                        },
-                        "indexOrAcceptablePremium": 0,
-                        "data": "0x0000000000000000000000000000000000000000",
-                    },
-                    {
-                        "actionType": ActionType.MINT_SHORT_OPTION.value,
-                        "owner": self.to_checksum_address(self._crypto.address),
-                        "secondAddress": self.to_checksum_address(
-                            self.web3_client.option_exchange.address
-                        ),
-                        "asset": self.to_checksum_address(otoken_id),
-                        "vaultId": int(vault_id),
-                        "amount": 100000000,
-                        "optionSeries": {
-                            "expiration": 1,
-                            "strike": 1,
-                            "isPut": True,
-                            "underlying": NULL_ADDRESS,
-                            "strikeAsset": NULL_ADDRESS,
-                            "collateral": NULL_ADDRESS,
-                        },
-                        "indexOrAcceptablePremium": 0,
-                        "data": "0x0000000000000000000000000000000000000000",
-                    },
-                ],
-            },
-            {
-                "operation": 1,
-                "operationQueue": [
-                    {
-                        "actionType": int(ActionType.BURN_SHORT_OPTION.value),
-                        "owner": NULL_ADDRESS,
-                        "secondAddress": self.to_checksum_address(self._crypto.address),
-                        "asset": NULL_ADDRESS,
-                        "vaultId": int(0),
-                        "amount": int(_amount),
-                        "optionSeries": {
-                            "expiration": int(rysk_option_market.expiration),
-                            "strike": int(rysk_option_market.strike),
-                            "isPut": bool(rysk_option_market.is_put),
-                            "underlying": self.to_checksum_address(
-                                underlying  # type: ignore
-                            ),
-                            "strikeAsset": self.to_checksum_address(
-                                strike_asset  # type: ignore
-                            ),
-                            "collateral": self.to_checksum_address(
-                                collateral_asset.value  # type: ignore
-                            ),
-                        },
-                        "indexOrAcceptablePremium": int(
-                            rysk_option_market.ask * (1 - ALLOWED_SLIPPAGE)
-                        ),
-                        "data": "0x0000000000000000000000000000000000000000",
-                    }
-                ],
-            },
-        ]
+        # has allowcance incremented
+        allowance = contract.functions.allowance(
+            self._crypto.address,
+            self.web3_client.option_exchange.address,
+        ).call()
+        self._logger.info(f"Allowance is {allowance}")
+        otoken_address = self.web3_client.get_otoken(rysk_option_market.to_series())
 
-        if self._logger.level is logging.DEBUG:
-            self._logger.debug("Operate tuple is:")
-            print_json(data=operate_tuple)
+        operate_tuple = sell(
+            int(acceptable_premium * 0.95 * 1e2),
+            owner_address=self._crypto.address,  # pylint: disable=E1120
+            exchange_address=self.web3_client.option_exchange.address,
+            otoken_address=otoken_address,
+            amount=int(_amount),
+            vault_id=int(vault_id),
+            collateral=_amount,
+            rysk_option_market=rysk_option_market,
+            issue_new_vault=issue_new_vault,
+        )
+        if self._verbose:
+            self._logger.info("Operate tuple is:")
+            print_operate_tuple(operate_tuple)
 
         operate_txn = self.web3_client.option_exchange.functions.operate(
             operate_tuple
-        ).build_transaction({"from": self._crypto.address})
+        ).build_transaction(
+            {
+                **{
+                    "from": self._crypto.address,
+                },
+                **self.web3_client._default_tx_params,  # pylint: disable=W0212
+            }
+        )
         return operate_txn
 
     def watch_trades(self):
         """Watch trades."""
         self._logger.info("Watching trades...")
         self.web3_client.watch_trades()
 
@@ -598,8 +567,122 @@
         self._logger.info("Fetching balances...")
         return self.web3_client.get_balances()
 
     def settle_vault(self, vault_id):
         """Settle options."""
         self._logger.info(f"Settling vault {vault_id}...")
         txn = self.web3_client.settle_vault(vault_id=vault_id)
-        return self.web3_client.sign_and_sumbit(txn, self._crypto.private_key)
+        return self._sign_and_sumbit(txn)
+
+    def redeem_otoken(self, otoken_id: str, amount: int):
+        """Redeem otoken."""
+        self._logger.info(f"Redeeming otoken {otoken_id}...")
+        txn = self.web3_client.redeem_otoken(otoken_id=otoken_id, amount=amount)
+        return self._sign_and_sumbit(txn)
+
+    def redeem_market(self, market: str):
+        """Redeem otoken."""
+        self._logger.info(f"Redeeming market {market}...")
+        rysk_option_market = RyskOptionMarket.from_str(market)
+        otoken_address = self.web3_client.get_otoken(rysk_option_market.to_series())
+        amount = self.web3_client.get_otoken_balance(otoken_address) / 10**8
+        return self.redeem_otoken(otoken_address, amount)
+
+    @property
+    def active_markets(self):
+        """Get active markets."""
+        if not self._markets:
+            self.fetch_markets()
+        return {market.name: market for market in self._markets}
+
+    def close_long(self, market: str, size: float):
+        """Close long."""
+        self._logger.info(f"Closing long {market}...")
+        # as we are long, we use usdc as collateral
+        collateral_asset = Collateral.USDC
+        _market = self.get_market(market)
+        _market.collateral = collateral_asset
+        otoken_address = self.web3_client.get_otoken(_market.to_series())
+        if size is None:
+            _amount = self.web3_client.get_otoken_balance(otoken_address) * 10**10
+        else:
+            _amount = size * 1e18
+        if _market.name not in self.active_markets:
+            raise ValueError(f"{market} is not an active market...")
+        acceptable_premium = int(_market.ask * (1 - ALLOWED_SLIPPAGE))
+        # we check the approval
+        otoken_contract = self.web3_client.get_otoken_contract(otoken_address)
+
+        # we get the balance
+        balance = self.web3_client.get_otoken_balance(otoken_address)
+
+        self._logger.info(f"Balance for {market} is {balance / 10**8}")
+
+        if balance == 0:
+            raise ValueError(f"Nothing to close for {market}...")
+
+        if not self.web3_client.is_approved(
+            otoken_contract,
+            self.web3_client.option_exchange.address,
+            self._crypto.address,
+            int(10**8 * _amount),
+        ):
+            self._logger.info(f"Approving {market}...")
+            txn = self.web3_client.create_approval(
+                otoken_contract,
+                self.web3_client.option_exchange.address,
+                self._crypto.address,  # type: ignore
+                int(10**8 * _amount),
+            )
+            self._sign_and_sumbit(
+                txn,
+            )
+
+        if _amount == 0:
+            raise ValueError(f"Nothing to close for {market}...")
+
+        txn = self.web3_client.close_long(
+            acceptable_premium=acceptable_premium,
+            amount=_amount,
+            otoken_address=self.web3_client.web3.toChecksumAddress(otoken_address),
+        )
+        return self._sign_and_sumbit(txn)
+
+    def close_short(self, market: str, size: float):
+        """
+        CLose short.
+        """
+        self._logger.info(f"Closing short {market}...")
+        # as we are short, we ensure we are covered
+        rysk_option_market = self.active_markets[market]
+        otoken_address = self.web3_client.get_otoken(rysk_option_market.to_series())
+
+        if size is None:
+            raise NotImplementedError(
+                "Closing short with no size is not implemented yet"
+            )
+        _amount = size * 1e18
+        if rysk_option_market.name not in self.active_markets:
+            raise ValueError(f"{market} is not an active market...")
+        acceptable_premium = int(rysk_option_market.bid * (1 + ALLOWED_SLIPPAGE) * size)
+
+        user_vaults = self.web3_client.fetch_user_vaults(self._crypto.address)
+        otoken_id = self.web3_client.get_otoken(rysk_option_market.to_series())
+        self._logger.info(f"Option Otoken id is {otoken_id}")
+
+        positions = [f for f in user_vaults if f[1] == otoken_id]
+        if len(positions) == 0:
+            raise ValueError(f"Nothing to close for {market}...")
+        if len(positions) > 1:
+            raise ValueError(f"Multiple positions for {market}...")
+        vault_id = positions[0][0]
+
+        txn = self.web3_client.close_short(
+            acceptable_premium=acceptable_premium,
+            amount=int(_amount),
+            otoken_address=self.web3_client.web3.toChecksumAddress(otoken_address),
+            collateral_asset=rysk_option_market.collateral,
+            collateral_amount=int(_amount),
+            vault_id=vault_id,
+            rysk_option_market=rysk_option_market,
+        )
+        return self._sign_and_sumbit(txn)
```

### Comparing `rysk_client-0.2.1/rysk_client/contracts/interfaces/AggregatorV3Interface.sol/AggregatorV3Interface.json` & `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4090520833333333%*

 * *Differences: {"'_format'": "''",*

 * * "'abi'": "{0: {'inputs': [OrderedDict([('internalType', 'address'), ('name', '_addressbook'), "*

 * *          "('type', 'address')])], 'stateMutability': 'nonpayable', 'type': 'constructor', delete: "*

 * *          "['name', 'outputs']}, 1: {'name': 'addressbook', 'outputs': {0: {'internalType': "*

 * *          "'contract AddressBookInterface', 'type': 'address'}}}, 2: {'inputs': {0: "*

 * *          "{'internalType': 'address', 'name': 'user', 'type': 'address'}}, 'name': "*

 * *          "'getVaultsForUser […]*

```diff
@@ -1,122 +1,88 @@
 {
-    "_format": "hh-sol-artifact-1",
+    "_format": "",
     "abi": [
         {
-            "inputs": [],
-            "name": "decimals",
-            "outputs": [
+            "inputs": [
                 {
-                    "internalType": "uint8",
-                    "name": "",
-                    "type": "uint8"
+                    "internalType": "address",
+                    "name": "_addressbook",
+                    "type": "address"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "stateMutability": "nonpayable",
+            "type": "constructor"
         },
         {
             "inputs": [],
-            "name": "description",
+            "name": "addressbook",
             "outputs": [
                 {
-                    "internalType": "string",
+                    "internalType": "contract AddressBookInterface",
                     "name": "",
-                    "type": "string"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "uint80",
-                    "name": "_roundId",
-                    "type": "uint80"
+                    "internalType": "address",
+                    "name": "user",
+                    "type": "address"
                 }
             ],
-            "name": "getRoundData",
+            "name": "getVaultsForUser",
             "outputs": [
                 {
-                    "internalType": "uint80",
-                    "name": "roundId",
-                    "type": "uint80"
-                },
-                {
-                    "internalType": "int256",
-                    "name": "answer",
-                    "type": "int256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "startedAt",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "updatedAt",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint80",
-                    "name": "answeredInRound",
-                    "type": "uint80"
+                    "components": [
+                        {
+                            "internalType": "uint256",
+                            "name": "vaultId",
+                            "type": "uint256"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "otoken",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct UserPositionLensMK1.VaultDrill[]",
+                    "name": "",
+                    "type": "tuple[]"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "latestRoundData",
-            "outputs": [
-                {
-                    "internalType": "uint80",
-                    "name": "roundId",
-                    "type": "uint80"
-                },
-                {
-                    "internalType": "int256",
-                    "name": "answer",
-                    "type": "int256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "startedAt",
-                    "type": "uint256"
-                },
+            "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "updatedAt",
-                    "type": "uint256"
+                    "internalType": "address",
+                    "name": "user",
+                    "type": "address"
                 },
                 {
-                    "internalType": "uint80",
-                    "name": "answeredInRound",
-                    "type": "uint80"
+                    "internalType": "address",
+                    "name": "otoken",
+                    "type": "address"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "version",
+            "name": "getVaultsForUserAndOtoken",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         }
     ],
-    "bytecode": "0x",
-    "contractName": "AggregatorV3Interface",
-    "deployedBytecode": "0x",
-    "deployedLinkReferences": {},
-    "linkReferences": {},
-    "sourceName": "contracts/interfaces/AggregatorV3Interface.sol"
+    "bytecode": "",
+    "deployedBytecode": "",
+    "deployedLinkReferences": "",
+    "sourceName": ""
 }
```

### Comparing `rysk_client-0.2.1/rysk_client/contracts/interfaces/IGmxVault.sol/IGmxVault.json` & `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.40169513378267974%*

 * *Differences: {"'_format'": "''",*

 * * "'abi'": "{0: {'inputs': {3: {'internalType': 'address', 'name': '_authority', 'type': "*

 * *          "'address'}, insert: [(0, OrderedDict([('internalType', 'address'), ('name', "*

 * *          "'_collateralAsset'), ('type', 'address')])), (1, OrderedDict([('internalType', "*

 * *          "'address'), ('name', '_liquidityPool'), ('type', 'address')])), (2, "*

 * *          "OrderedDict([('internalType', 'address'), ('name', '_addressBook'), ('type', "*

 * *          "'address')]))]}, 'stateMutability': 'no […]*

```diff
@@ -1,1726 +1,1267 @@
 {
-    "_format": "hh-sol-artifact-1",
+    "_format": "",
     "abi": [
         {
             "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "name": "allWhitelistedTokens",
-            "outputs": [
-                {
                     "internalType": "address",
-                    "name": "",
-                    "type": "address"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "allWhitelistedTokensLength",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_account",
+                    "name": "_collateralAsset",
                     "type": "address"
                 },
                 {
                     "internalType": "address",
-                    "name": "_router",
-                    "type": "address"
-                }
-            ],
-            "name": "approvedRouters",
-            "outputs": [
-                {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
+                    "name": "_liquidityPool",
                     "type": "address"
-                }
-            ],
-            "name": "bufferAmounts",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                },
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_addressBook",
                     "type": "address"
                 },
                 {
                     "internalType": "address",
-                    "name": "_receiver",
+                    "name": "_authority",
                     "type": "address"
                 }
             ],
-            "name": "buyUSDG",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
             "stateMutability": "nonpayable",
-            "type": "function"
+            "type": "constructor"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "cumulativeFundingRates",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
+            "inputs": [],
+            "name": "AlreadyExpired",
+            "type": "error"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_account",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_collateralToken",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_collateralDelta",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_sizeDelta",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_receiver",
-                    "type": "address"
-                }
-            ],
-            "name": "decreasePosition",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "nonpayable",
-            "type": "function"
+            "inputs": [],
+            "name": "HealthyVault",
+            "type": "error"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "directPoolDeposit",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
+            "inputs": [],
+            "name": "InsufficientBalance",
+            "type": "error"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "feeReserves",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
+            "inputs": [],
+            "name": "InvalidCollateral",
+            "type": "error"
         },
         {
             "inputs": [],
-            "name": "fundingInterval",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "InvalidDecimals",
+            "type": "error"
         },
         {
             "inputs": [],
-            "name": "fundingRateFactor",
-            "outputs": [
+            "name": "NoVault",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "NonExistentSeries",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "NotExpired",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "NotKeeper",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "NotLiquidityPool",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "NotOperator",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "SeriesAddressAlreadySet",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "SeriesInfoAlreadySet",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "UNAUTHORIZED",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "VaultAlreadySet",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "VaultExpired",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "VaultNotLiquidated",
+            "type": "error"
+        },
+        {
+            "inputs": [],
+            "name": "WithdrawExceedsLiquidity",
+            "type": "error"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "indexed": false,
+                    "internalType": "contract IAuthority",
+                    "name": "authority",
+                    "type": "address"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "AuthorityUpdated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
+                    "indexed": false,
+                    "internalType": "uint64",
+                    "name": "putLower",
+                    "type": "uint64"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "_size",
-                    "type": "uint256"
+                    "indexed": false,
+                    "internalType": "uint64",
+                    "name": "putUpper",
+                    "type": "uint64"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "_averagePrice",
-                    "type": "uint256"
+                    "indexed": false,
+                    "internalType": "uint64",
+                    "name": "callLower",
+                    "type": "uint64"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_lastIncreasedTime",
-                    "type": "uint256"
-                }
-            ],
-            "name": "getDelta",
-            "outputs": [
-                {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "indexed": false,
+                    "internalType": "uint64",
+                    "name": "callUpper",
+                    "type": "uint64"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "HealthThresholdsUpdated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": false,
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "target",
                     "type": "address"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "_usdgDelta",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_feeBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_taxBasisPoints",
-                    "type": "uint256"
-                },
-                {
+                    "indexed": false,
                     "internalType": "bool",
-                    "name": "_increment",
+                    "name": "auth",
                     "type": "bool"
                 }
             ],
-            "name": "getFeeBasisPoints",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "KeeperUpdated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": false,
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "newLiquidityPool",
                     "type": "address"
                 }
             ],
-            "name": "getMaxPrice",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "LiquidityPoolUpdated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": false,
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "operator",
                     "type": "address"
-                }
-            ],
-            "name": "getMinPrice",
-            "outputs": [
+                },
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "indexed": false,
+                    "internalType": "bool",
+                    "name": "isOperator",
+                    "type": "bool"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "OperatorUpdated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": false,
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "token",
                     "type": "address"
                 }
             ],
-            "name": "getNextFundingRate",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "OptionTokenCreated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": true,
                     "internalType": "address",
-                    "name": "_account",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_collateralToken",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_indexToken",
+                    "name": "series",
                     "type": "address"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
-                }
-            ],
-            "name": "getPosition",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                },
-                {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "vaultId",
                     "type": "uint256"
                 },
                 {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "closedAmount",
                     "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                },
+                }
+            ],
+            "name": "OptionsContractClosed",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "indexed": true,
+                    "internalType": "address",
+                    "name": "series",
+                    "type": "address"
                 },
                 {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "vaultId",
                     "type": "uint256"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
-                },
-                {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "optionsAmount",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "OptionsContractOpened",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": true,
                     "internalType": "address",
-                    "name": "_account",
+                    "name": "series",
                     "type": "address"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_collateralToken",
-                    "type": "address"
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "collateralReturned",
+                    "type": "uint256"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "collateralLost",
+                    "type": "uint256"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
-                }
-            ],
-            "name": "getPositionKey",
-            "outputs": [
-                {
-                    "internalType": "bytes32",
-                    "name": "",
-                    "type": "bytes32"
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "amountLost",
+                    "type": "uint256"
                 }
             ],
-            "stateMutability": "pure",
-            "type": "function"
+            "name": "OptionsContractSettled",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": false,
                     "internalType": "address",
-                    "name": "_account",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_collateralToken",
+                    "name": "series",
                     "type": "address"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "underlyingAmount",
+                    "type": "uint256"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
-                }
-            ],
-            "name": "getPositionLeverage",
-            "outputs": [
-                {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "strikeAmount",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "SeriesRedeemed",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": true,
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "series",
                     "type": "address"
                 },
                 {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "_usdgAmount",
+                    "name": "vaultId",
                     "type": "uint256"
-                }
-            ],
-            "name": "getRedemptionAmount",
-            "outputs": [
+                },
                 {
+                    "indexed": false,
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "amountLiquidated",
+                    "type": "uint256"
+                },
+                {
+                    "indexed": false,
+                    "internalType": "uint256",
+                    "name": "collateralLiquidated",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "name": "VaultLiquidationRegistered",
+            "type": "event"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "getTargetUsdgAmount",
+            "inputs": [],
+            "name": "addressBook",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "contract AddressBookInterface",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "globalShortAveragePrices",
-            "outputs": [
-                {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "vaultId",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "name": "adjustCollateral",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "globalShortSizes",
-            "outputs": [
-                {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "vaultId",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "name": "adjustCollateralCaller",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "gov",
+            "name": "authority",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "contract IAuthority",
                     "name": "",
                     "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "guaranteedUsd",
+            "inputs": [],
+            "name": "callLowerHealthFactor",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "uint64",
                     "name": "",
-                    "type": "uint256"
+                    "type": "uint64"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "hasDynamicFees",
+            "name": "callUpperHealthFactor",
             "outputs": [
                 {
-                    "internalType": "bool",
+                    "internalType": "uint64",
                     "name": "",
-                    "type": "bool"
+                    "type": "uint64"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "inManagerMode",
-            "outputs": [
+            "inputs": [
                 {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
+                    "internalType": "uint256",
+                    "name": "vaultId",
+                    "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "inPrivateLiquidationMode",
+            "name": "checkVaultHealth",
             "outputs": [
                 {
                     "internalType": "bool",
-                    "name": "",
+                    "name": "isBelowMin",
                     "type": "bool"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                },
                 {
-                    "internalType": "address",
-                    "name": "_account",
-                    "type": "address"
+                    "internalType": "bool",
+                    "name": "isAboveMax",
+                    "type": "bool"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_collateralToken",
-                    "type": "address"
+                    "internalType": "uint256",
+                    "name": "healthFactor",
+                    "type": "uint256"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
+                    "internalType": "uint256",
+                    "name": "upperHealthFactor",
+                    "type": "uint256"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "_sizeDelta",
+                    "name": "collatRequired",
                     "type": "uint256"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
+                    "internalType": "address",
+                    "name": "collatAsset",
+                    "type": "address"
                 }
             ],
-            "name": "increasePosition",
-            "outputs": [],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "isInitialized",
-            "outputs": [
+            "inputs": [
                 {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
+                    "internalType": "address",
+                    "name": "_series",
+                    "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "amount",
+                    "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "isLeverageEnabled",
+            "name": "close",
             "outputs": [
                 {
                     "internalType": "bool",
                     "name": "",
                     "type": "bool"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "",
+                    "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_account",
-                    "type": "address"
-                }
-            ],
-            "name": "isLiquidator",
+            "inputs": [],
+            "name": "collateralAsset",
             "outputs": [
                 {
-                    "internalType": "bool",
+                    "internalType": "address",
                     "name": "",
-                    "type": "bool"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_account",
-                    "type": "address"
-                }
-            ],
-            "name": "isManager",
-            "outputs": [
+                    "components": [
+                        {
+                            "internalType": "uint64",
+                            "name": "expiration",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint128",
+                            "name": "strike",
+                            "type": "uint128"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "isPut",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "underlying",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "strikeAsset",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "collateral",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct Types.OptionSeries",
+                    "name": "series",
+                    "type": "tuple"
+                },
                 {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
+                    "internalType": "uint256",
+                    "name": "amount",
+                    "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "isSwapEnabled",
+            "name": "getCollateral",
             "outputs": [
                 {
-                    "internalType": "bool",
+                    "internalType": "uint256",
                     "name": "",
-                    "type": "bool"
+                    "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
+                    "components": [
+                        {
+                            "internalType": "uint64",
+                            "name": "expiration",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint128",
+                            "name": "strike",
+                            "type": "uint128"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "isPut",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "underlying",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "strikeAsset",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "collateral",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct Types.OptionSeries",
+                    "name": "_series",
+                    "type": "tuple"
                 }
             ],
-            "name": "lastFundingTimes",
+            "name": "getIssuanceHash",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bytes32",
                     "name": "",
-                    "type": "uint256"
+                    "type": "bytes32"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "pure",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_account",
+                    "name": "underlying",
                     "type": "address"
                 },
                 {
                     "internalType": "address",
-                    "name": "_collateralToken",
+                    "name": "strikeAsset",
                     "type": "address"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
+                    "internalType": "uint256",
+                    "name": "expiration",
+                    "type": "uint256"
                 },
                 {
                     "internalType": "bool",
-                    "name": "_isLong",
+                    "name": "isPut",
                     "type": "bool"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_feeReceiver",
-                    "type": "address"
-                }
-            ],
-            "name": "liquidatePosition",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "liquidationFeeUsd",
-            "outputs": [
-                {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "strike",
                     "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "marginFeeBasisPoints",
-            "outputs": [
+                },
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "internalType": "address",
+                    "name": "collateral",
+                    "type": "address"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "maxGasPrice",
+            "name": "getOtoken",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
+                    "components": [
+                        {
+                            "internalType": "uint64",
+                            "name": "expiration",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint128",
+                            "name": "strike",
+                            "type": "uint128"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "isPut",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "underlying",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "strikeAsset",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "collateral",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct Types.OptionSeries",
+                    "name": "_series",
+                    "type": "tuple"
                 }
             ],
-            "name": "maxGlobalShortSizes",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "maxLeverage",
+            "name": "getSeries",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
+                    "internalType": "bytes32",
+                    "name": "issuanceHash",
+                    "type": "bytes32"
                 }
             ],
-            "name": "maxUsdgAmounts",
+            "name": "getSeriesAddress",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "series",
                     "type": "address"
                 }
             ],
-            "name": "minProfitBasisPoints",
+            "name": "getSeriesInfo",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "components": [
+                        {
+                            "internalType": "uint64",
+                            "name": "expiration",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint128",
+                            "name": "strike",
+                            "type": "uint128"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "isPut",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "underlying",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "strikeAsset",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "collateral",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct Types.OptionSeries",
                     "name": "",
-                    "type": "uint256"
+                    "type": "tuple"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "minProfitTime",
-            "outputs": [
+            "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "components": [
+                        {
+                            "internalType": "uint64",
+                            "name": "expiration",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint128",
+                            "name": "strike",
+                            "type": "uint128"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "isPut",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "underlying",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "strikeAsset",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "collateral",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct Types.OptionSeries",
+                    "name": "optionSeries",
+                    "type": "tuple"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "mintBurnFeeBasisPoints",
+            "name": "issue",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "",
                     "type": "address"
                 }
             ],
-            "name": "poolAmounts",
+            "name": "keeper",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "uint256"
+                    "type": "bool"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "priceFeed",
+            "name": "liquidityPool",
             "outputs": [
                 {
                     "internalType": "address",
                     "name": "",
                     "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_series",
                     "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "amount",
+                    "type": "uint256"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "collateralAmount",
+                    "type": "uint256"
                 }
             ],
-            "name": "reservedAmounts",
+            "name": "open",
             "outputs": [
                 {
+                    "internalType": "bool",
+                    "name": "",
+                    "type": "bool"
+                },
+                {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "router",
+            "name": "putLowerHealthFactor",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "uint64",
                     "name": "",
-                    "type": "address"
+                    "type": "uint64"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_receiver",
-                    "type": "address"
-                }
-            ],
-            "name": "sellUSDG",
+            "inputs": [],
+            "name": "putUpperHealthFactor",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "uint64",
                     "name": "",
-                    "type": "uint256"
+                    "type": "uint64"
                 }
             ],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_series",
                     "type": "address"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_amount",
-                    "type": "uint256"
-                }
-            ],
-            "name": "setBufferAmount",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "_errorCode",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "string",
-                    "name": "_error",
-                    "type": "string"
                 }
             ],
-            "name": "setError",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "_taxBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_stableTaxBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_mintBurnFeeBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_swapFeeBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_stableSwapFeeBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_marginFeeBasisPoints",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_liquidationFeeUsd",
-                    "type": "uint256"
-                },
+            "name": "redeem",
+            "outputs": [
                 {
                     "internalType": "uint256",
-                    "name": "_minProfitTime",
+                    "name": "",
                     "type": "uint256"
-                },
-                {
-                    "internalType": "bool",
-                    "name": "_hasDynamicFees",
-                    "type": "bool"
                 }
             ],
-            "name": "setFees",
-            "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "uint256",
-                    "name": "_fundingInterval",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_fundingRateFactor",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_stableFundingRateFactor",
+                    "name": "vaultId",
                     "type": "uint256"
                 }
             ],
-            "name": "setFundingRate",
+            "name": "registerLiquidatedVault",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "bool",
-                    "name": "_inManagerMode",
-                    "type": "bool"
+                    "internalType": "address",
+                    "name": "",
+                    "type": "address"
                 }
             ],
-            "name": "setInManagerMode",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
+            "name": "seriesInfo",
+            "outputs": [
                 {
-                    "internalType": "bool",
-                    "name": "_inPrivateLiquidationMode",
-                    "type": "bool"
-                }
-            ],
-            "name": "setInPrivateLiquidationMode",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                    "internalType": "uint64",
+                    "name": "expiration",
+                    "type": "uint64"
+                },
                 {
-                    "internalType": "bool",
-                    "name": "_isLeverageEnabled",
-                    "type": "bool"
-                }
-            ],
-            "name": "setIsLeverageEnabled",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                    "internalType": "uint128",
+                    "name": "strike",
+                    "type": "uint128"
+                },
                 {
                     "internalType": "bool",
-                    "name": "_isSwapEnabled",
+                    "name": "isPut",
                     "type": "bool"
-                }
-            ],
-            "name": "setIsSwapEnabled",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                },
                 {
                     "internalType": "address",
-                    "name": "_liquidator",
+                    "name": "underlying",
                     "type": "address"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isActive",
-                    "type": "bool"
-                }
-            ],
-            "name": "setLiquidator",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
                     "internalType": "address",
-                    "name": "_manager",
+                    "name": "strikeAsset",
                     "type": "address"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isManager",
-                    "type": "bool"
-                }
-            ],
-            "name": "setManager",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "_maxGasPrice",
-                    "type": "uint256"
-                }
-            ],
-            "name": "setMaxGasPrice",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "collateral",
                     "type": "address"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_amount",
-                    "type": "uint256"
                 }
             ],
-            "name": "setMaxGlobalShortSize",
-            "outputs": [],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "_maxLeverage",
-                    "type": "uint256"
-                }
-            ],
-            "name": "setMaxLeverage",
-            "outputs": [],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_priceFeed",
+                    "internalType": "contract IAuthority",
+                    "name": "_newAuthority",
                     "type": "address"
                 }
             ],
-            "name": "setPriceFeed",
+            "name": "setAuthority",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
+                    "internalType": "uint64",
+                    "name": "_putLower",
+                    "type": "uint64"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "_tokenDecimals",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_redemptionBps",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_minProfitBps",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_maxUsdgAmount",
-                    "type": "uint256"
+                    "internalType": "uint64",
+                    "name": "_putUpper",
+                    "type": "uint64"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isStable",
-                    "type": "bool"
+                    "internalType": "uint64",
+                    "name": "_callLower",
+                    "type": "uint64"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "_isShortable",
-                    "type": "bool"
+                    "internalType": "uint64",
+                    "name": "_callUpper",
+                    "type": "uint64"
                 }
             ],
-            "name": "setTokenConfig",
+            "name": "setHealthThresholds",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_target",
                     "type": "address"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "_amount",
-                    "type": "uint256"
+                    "internalType": "bool",
+                    "name": "_auth",
+                    "type": "bool"
                 }
             ],
-            "name": "setUsdgAmount",
+            "name": "setKeeper",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_newLiquidityPool",
                     "type": "address"
                 }
             ],
-            "name": "shortableTokens",
-            "outputs": [
-                {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "stableFundingRateFactor",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "stableSwapFeeBasisPoints",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "stableTaxBasisPoints",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
+            "name": "setLiquidityPool",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_operator",
                     "type": "address"
-                }
-            ],
-            "name": "stableTokens",
-            "outputs": [
+                },
                 {
                     "internalType": "bool",
-                    "name": "",
+                    "name": "_isOperator",
                     "type": "bool"
                 }
             ],
-            "stateMutability": "view",
+            "name": "setOperator",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_tokenIn",
-                    "type": "address"
+                    "components": [
+                        {
+                            "internalType": "uint64",
+                            "name": "expiration",
+                            "type": "uint64"
+                        },
+                        {
+                            "internalType": "uint128",
+                            "name": "strike",
+                            "type": "uint128"
+                        },
+                        {
+                            "internalType": "bool",
+                            "name": "isPut",
+                            "type": "bool"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "underlying",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "strikeAsset",
+                            "type": "address"
+                        },
+                        {
+                            "internalType": "address",
+                            "name": "collateral",
+                            "type": "address"
+                        }
+                    ],
+                    "internalType": "struct Types.OptionSeries",
+                    "name": "_optionSeries",
+                    "type": "tuple"
                 },
                 {
                     "internalType": "address",
-                    "name": "_tokenOut",
+                    "name": "_seriesAddress",
                     "type": "address"
                 },
                 {
-                    "internalType": "address",
-                    "name": "_receiver",
-                    "type": "address"
-                }
-            ],
-            "name": "swap",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "internalType": "bytes32",
+                    "name": "_issuanceHash",
+                    "type": "bytes32"
                 }
             ],
+            "name": "setSeriesInfoAndAddress",
+            "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "swapFeeBasisPoints",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "taxBasisPoints",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_seriesAddress",
                     "type": "address"
-                }
-            ],
-            "name": "tokenBalances",
-            "outputs": [
+                },
                 {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "_id",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "name": "setVaultIds",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
+                    "name": "_series",
                     "type": "address"
                 }
             ],
-            "name": "tokenDecimals",
+            "name": "settle",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
+                    "type": "bool"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "_tokenAmount",
-                    "type": "uint256"
-                }
-            ],
-            "name": "tokenToUsdMin",
-            "outputs": [
-                {
-                    "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "tokenWeights",
-            "outputs": [
+                },
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "totalTokenWeights",
-            "outputs": [
+                },
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "usdg",
+            "name": "vaultCount",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "uint64",
                     "name": "",
-                    "type": "address"
+                    "type": "uint64"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "usdgAmounts",
-            "outputs": [
-                {
-                    "internalType": "uint256",
                     "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_account",
                     "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_collateralToken",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_indexToken",
-                    "type": "address"
-                },
-                {
-                    "internalType": "bool",
-                    "name": "_isLong",
-                    "type": "bool"
-                },
-                {
-                    "internalType": "bool",
-                    "name": "_raise",
-                    "type": "bool"
-                }
-            ],
-            "name": "validateLiquidation",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "whitelistedTokenCount",
+            "name": "vaultIds",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                }
-            ],
-            "name": "whitelistedTokens",
-            "outputs": [
-                {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "_token",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_receiver",
-                    "type": "address"
-                }
-            ],
-            "name": "withdrawFees",
-            "outputs": [
-                {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "vaultId",
                     "type": "uint256"
                 }
             ],
+            "name": "wCollatLiquidatedVault",
+            "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "bytecode": "0x",
-    "contractName": "IGmxVault",
-    "deployedBytecode": "0x",
-    "deployedLinkReferences": {},
-    "linkReferences": {},
-    "sourceName": "contracts/interfaces/IGmxVault.sol"
+    "bytecode": "",
+    "deployedBytecode": "",
+    "deployedLinkReferences": "",
+    "sourceName": ""
 }
```

### Comparing `rysk_client-0.2.1/rysk_client/contracts/interfaces/ILiquidityPool.sol/ILiquidityPool.json` & `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4128795295530493%*

 * *Differences: {"'_format'": "''",*

 * * "'abi'": "{2: {'inputs': [], 'name': 'DOMAIN_SEPARATOR', 'outputs': "*

 * *          "[OrderedDict([('internalType', 'bytes32'), ('name', ''), ('type', 'bytes32')])], "*

 * *          "'stateMutability': 'view'}, 6: {'inputs': [OrderedDict([('internalType', 'address'), "*

 * *          "('name', 'account'), ('type', 'address')]), OrderedDict([('internalType', 'uint256'), "*

 * *          "('name', 'amount'), ('type', 'uint256')])], 'name': 'burnOtoken', 'outputs': [], "*

 * *          "'stateMutability': 'nonpa […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "_format": "hh-sol-artifact-1",
+    "_format": "",
     "abi": [
         {
             "anonymous": false,
             "inputs": [
                 {
                     "indexed": true,
                     "internalType": "address",
@@ -48,39 +48,24 @@
                     "type": "uint256"
                 }
             ],
             "name": "Transfer",
             "type": "event"
         },
         {
-            "inputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "collateralAmount",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "optionsValue",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "int256",
-                    "name": "delta",
-                    "type": "int256"
-                },
+            "inputs": [],
+            "name": "DOMAIN_SEPARATOR",
+            "outputs": [
                 {
-                    "internalType": "bool",
-                    "name": "isSale",
-                    "type": "bool"
+                    "internalType": "bytes32",
+                    "name": "",
+                    "type": "bytes32"
                 }
             ],
-            "name": "adjustVariables",
-            "outputs": [],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
                     "name": "owner",
@@ -143,50 +128,29 @@
                     "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "bufferPercentage",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "checkBuffer",
-            "outputs": [
+            "inputs": [
                 {
-                    "internalType": "int256",
-                    "name": "bufferRemaining",
-                    "type": "int256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "collateralAllocated",
-            "outputs": [
+                    "internalType": "address",
+                    "name": "account",
+                    "type": "address"
+                },
                 {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "amount",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "name": "burnOtoken",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
             "name": "collateralAsset",
             "outputs": [
                 {
@@ -196,610 +160,320 @@
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "collateralCap",
+            "name": "controller",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "depositEpoch",
+            "name": "decimals",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "uint8",
                     "name": "",
-                    "type": "uint256"
+                    "type": "uint8"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "epoch",
-                    "type": "uint256"
-                }
-            ],
-            "name": "depositEpochPricePerShare",
-            "outputs": [
+                    "internalType": "address",
+                    "name": "spender",
+                    "type": "address"
+                },
                 {
                     "internalType": "uint256",
-                    "name": "price",
+                    "name": "subtractedValue",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "depositor",
-                    "type": "address"
-                }
-            ],
-            "name": "depositReceipts",
+            "name": "decreaseAllowance",
             "outputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint128",
-                            "name": "epoch",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "amount",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "unredeemedShares",
-                            "type": "uint256"
-                        }
-                    ],
-                    "internalType": "struct IAccounting.DepositReceipt",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "tuple"
+                    "type": "bool"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "ephemeralDelta",
+            "name": "expiryTimestamp",
             "outputs": [
                 {
-                    "internalType": "int256",
+                    "internalType": "uint256",
                     "name": "",
-                    "type": "int256"
+                    "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "ephemeralLiabilities",
+            "name": "getOtokenDetails",
             "outputs": [
                 {
-                    "internalType": "int256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "int256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "getAssets",
-            "outputs": [
+                    "type": "address"
+                },
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                    "type": "address"
+                },
                 {
                     "internalType": "address",
-                    "name": "asset",
+                    "name": "",
                     "type": "address"
-                }
-            ],
-            "name": "getBalance",
-            "outputs": [
+                },
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "getPortfolioDelta",
-            "outputs": [
+                },
                 {
-                    "internalType": "int256",
+                    "internalType": "uint256",
                     "name": "",
-                    "type": "int256"
+                    "type": "uint256"
+                },
+                {
+                    "internalType": "bool",
+                    "name": "",
+                    "type": "bool"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "optionSeries",
-                    "type": "tuple"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "amount",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "contract IOptionRegistry",
-                    "name": "optionRegistry",
-                    "type": "address"
-                },
-                {
                     "internalType": "address",
-                    "name": "seriesAddress",
+                    "name": "spender",
                     "type": "address"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "premium",
+                    "name": "addedValue",
                     "type": "uint256"
-                },
-                {
-                    "internalType": "int256",
-                    "name": "delta",
-                    "type": "int256"
-                },
-                {
-                    "internalType": "address",
-                    "name": "seller",
-                    "type": "address"
                 }
             ],
-            "name": "handlerBuybackOption",
+            "name": "increaseAllowance",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "uint256"
+                    "type": "bool"
                 }
             ],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "optionSeries",
-                    "type": "tuple"
-                }
-            ],
-            "name": "handlerIssue",
-            "outputs": [
-                {
                     "internalType": "address",
-                    "name": "",
+                    "name": "_addressBook",
                     "type": "address"
-                }
-            ],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "optionSeries",
-                    "type": "tuple"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "amount",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "premium",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "int256",
-                    "name": "delta",
-                    "type": "int256"
                 },
                 {
                     "internalType": "address",
-                    "name": "recipient",
+                    "name": "_underlyingAsset",
                     "type": "address"
-                }
-            ],
-            "name": "handlerIssueAndWriteOption",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
                 },
                 {
                     "internalType": "address",
-                    "name": "",
+                    "name": "_strikeAsset",
                     "type": "address"
-                }
-            ],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "optionSeries",
-                    "type": "tuple"
                 },
                 {
                     "internalType": "address",
-                    "name": "seriesAddress",
+                    "name": "_collateralAsset",
                     "type": "address"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "amount",
+                    "name": "_strikePrice",
                     "type": "uint256"
                 },
                 {
-                    "internalType": "contract IOptionRegistry",
-                    "name": "optionRegistry",
-                    "type": "address"
-                },
-                {
                     "internalType": "uint256",
-                    "name": "premium",
+                    "name": "_expiryTimestamp",
                     "type": "uint256"
                 },
                 {
-                    "internalType": "int256",
-                    "name": "delta",
-                    "type": "int256"
-                },
-                {
-                    "internalType": "address",
-                    "name": "recipient",
-                    "type": "address"
+                    "internalType": "bool",
+                    "name": "_isPut",
+                    "type": "bool"
                 }
             ],
-            "name": "handlerWriteOption",
+            "name": "init",
+            "outputs": [],
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "isPut",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "uint256"
+                    "type": "bool"
                 }
             ],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "partitionedFunds",
-            "outputs": [
+            "inputs": [
+                {
+                    "internalType": "address",
+                    "name": "account",
+                    "type": "address"
+                },
                 {
                     "internalType": "uint256",
-                    "name": "",
+                    "name": "amount",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "view",
+            "name": "mintOtoken",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "pendingDeposits",
+            "name": "name",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "string",
                     "name": "",
-                    "type": "uint256"
+                    "type": "string"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
-            "name": "pendingWithdrawals",
+            "inputs": [
+                {
+                    "internalType": "address",
+                    "name": "owner",
+                    "type": "address"
+                }
+            ],
+            "name": "nonces",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "optionSeries",
-                    "type": "tuple"
+                    "internalType": "address",
+                    "name": "owner",
+                    "type": "address"
+                },
+                {
+                    "internalType": "address",
+                    "name": "spender",
+                    "type": "address"
                 },
                 {
                     "internalType": "uint256",
                     "name": "amount",
                     "type": "uint256"
                 },
                 {
-                    "internalType": "bool",
-                    "name": "toBuy",
-                    "type": "bool"
-                }
-            ],
-            "name": "quotePriceWithUtilizationGreeks",
-            "outputs": [
-                {
                     "internalType": "uint256",
-                    "name": "quote",
+                    "name": "deadline",
                     "type": "uint256"
                 },
                 {
-                    "internalType": "int256",
-                    "name": "delta",
-                    "type": "int256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
+                    "internalType": "uint8",
+                    "name": "v",
+                    "type": "uint8"
+                },
                 {
-                    "internalType": "int256",
-                    "name": "delta",
-                    "type": "int256"
+                    "internalType": "bytes32",
+                    "name": "r",
+                    "type": "bytes32"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "index",
-                    "type": "uint256"
+                    "internalType": "bytes32",
+                    "name": "s",
+                    "type": "bytes32"
                 }
             ],
-            "name": "rebalancePortfolioDelta",
+            "name": "permit",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
-            "inputs": [
+            "inputs": [],
+            "name": "strikeAsset",
+            "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "address",
                     "name": "",
-                    "type": "uint256"
+                    "type": "address"
                 }
             ],
-            "name": "redeem",
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "strikePrice",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
             ],
-            "stateMutability": "nonpayable",
-            "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "resetEphemeralValues",
-            "outputs": [],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "strikeAsset",
+            "name": "symbol",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "string",
                     "name": "",
-                    "type": "address"
+                    "type": "string"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
@@ -875,79 +549,14 @@
                     "internalType": "address",
                     "name": "",
                     "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
-        },
-        {
-            "inputs": [],
-            "name": "withdrawalEpoch",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "epoch",
-                    "type": "uint256"
-                }
-            ],
-            "name": "withdrawalEpochPricePerShare",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "price",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [
-                {
-                    "internalType": "address",
-                    "name": "withdrawer",
-                    "type": "address"
-                }
-            ],
-            "name": "withdrawalReceipts",
-            "outputs": [
-                {
-                    "components": [
-                        {
-                            "internalType": "uint128",
-                            "name": "epoch",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "shares",
-                            "type": "uint128"
-                        }
-                    ],
-                    "internalType": "struct IAccounting.WithdrawalReceipt",
-                    "name": "",
-                    "type": "tuple"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
         }
     ],
-    "bytecode": "0x",
-    "contractName": "ILiquidityPool",
-    "deployedBytecode": "0x",
-    "deployedLinkReferences": {},
-    "linkReferences": {},
-    "sourceName": "contracts/interfaces/ILiquidityPool.sol"
+    "bytecode": "",
+    "deployedBytecode": "",
+    "deployedLinkReferences": "",
+    "sourceName": ""
 }
```

### Comparing `rysk_client-0.2.1/rysk_client/contracts/interfaces/IOptionRegistry.sol/IOptionRegistry.json` & `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3993266369047619%*

 * *Differences: {"'_format'": "''",*

 * * "'abi'": "{5: {'name': 'DOMAIN_SEPARATOR', 'outputs': {0: {'internalType': 'bytes32', 'type': "*

 * *          "'bytes32'}}}, 7: {'inputs': {0: {'name': 'spender'}}, 'name': 'approve', 'outputs': "*

 * *          "{delete: [1]}}, 9: {'inputs': {0: {'internalType': 'address', 'name': '', 'type': "*

 * *          "'address'}, delete: [0]}, 'name': 'balanceOf'}, 10: {'inputs': [], 'name': 'decimals', "*

 * *          "'outputs': {0: {'internalType': 'uint8', 'type': 'uint8'}}}, 12: {'inputs': [], 'name': "*

 * *   […]*

```diff
@@ -1,393 +1,400 @@
 {
-    "_format": "hh-sol-artifact-1",
+    "_format": "",
     "abi": [
         {
-            "inputs": [],
-            "name": "addressBook",
-            "outputs": [
+            "inputs": [
+                {
+                    "internalType": "string",
+                    "name": "_name",
+                    "type": "string"
+                },
+                {
+                    "internalType": "string",
+                    "name": "_symbol",
+                    "type": "string"
+                },
+                {
+                    "internalType": "uint8",
+                    "name": "_decimals",
+                    "type": "uint8"
+                },
                 {
                     "internalType": "address",
-                    "name": "",
+                    "name": "_authority",
                     "type": "address"
                 }
             ],
-            "stateMutability": "view",
-            "type": "function"
+            "stateMutability": "nonpayable",
+            "type": "constructor"
         },
         {
+            "inputs": [],
+            "name": "UNAUTHORIZED",
+            "type": "error"
+        },
+        {
+            "anonymous": false,
             "inputs": [
                 {
+                    "indexed": true,
+                    "internalType": "address",
+                    "name": "owner",
+                    "type": "address"
+                },
+                {
+                    "indexed": true,
                     "internalType": "address",
-                    "name": "_series",
+                    "name": "spender",
                     "type": "address"
                 },
                 {
+                    "indexed": false,
                     "internalType": "uint256",
                     "name": "amount",
                     "type": "uint256"
                 }
             ],
-            "name": "close",
-            "outputs": [
-                {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
-                },
+            "name": "Approval",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "indexed": false,
+                    "internalType": "contract IAuthority",
+                    "name": "authority",
+                    "type": "address"
                 }
             ],
-            "stateMutability": "nonpayable",
-            "type": "function"
+            "name": "AuthorityUpdated",
+            "type": "event"
         },
         {
+            "anonymous": false,
             "inputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "series",
-                    "type": "tuple"
+                    "indexed": true,
+                    "internalType": "address",
+                    "name": "from",
+                    "type": "address"
+                },
+                {
+                    "indexed": true,
+                    "internalType": "address",
+                    "name": "to",
+                    "type": "address"
                 },
                 {
+                    "indexed": false,
                     "internalType": "uint256",
                     "name": "amount",
                     "type": "uint256"
                 }
             ],
-            "name": "getCollateral",
+            "name": "Transfer",
+            "type": "event"
+        },
+        {
+            "inputs": [],
+            "name": "DOMAIN_SEPARATOR",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bytes32",
                     "name": "",
-                    "type": "uint256"
+                    "type": "bytes32"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "underlying",
+                    "name": "",
                     "type": "address"
                 },
                 {
                     "internalType": "address",
-                    "name": "strikeAsset",
+                    "name": "",
                     "type": "address"
-                },
+                }
+            ],
+            "name": "allowance",
+            "outputs": [
                 {
                     "internalType": "uint256",
-                    "name": "expiration",
+                    "name": "",
                     "type": "uint256"
-                },
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
                 {
-                    "internalType": "bool",
-                    "name": "isPut",
-                    "type": "bool"
+                    "internalType": "address",
+                    "name": "spender",
+                    "type": "address"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "strike",
+                    "name": "amount",
                     "type": "uint256"
-                },
+                }
+            ],
+            "name": "approve",
+            "outputs": [
                 {
-                    "internalType": "address",
-                    "name": "collateral",
-                    "type": "address"
+                    "internalType": "bool",
+                    "name": "",
+                    "type": "bool"
                 }
             ],
-            "name": "getOtoken",
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "authority",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "contract IAuthority",
                     "name": "",
                     "type": "address"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "_series",
-                    "type": "tuple"
+                    "internalType": "address",
+                    "name": "",
+                    "type": "address"
                 }
             ],
-            "name": "getSeries",
+            "name": "balanceOf",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "uint256",
                     "name": "",
-                    "type": "address"
+                    "type": "uint256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "decimals",
+            "outputs": [
+                {
+                    "internalType": "uint8",
+                    "name": "",
+                    "type": "uint8"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "series",
+                    "name": "to",
                     "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "amount",
+                    "type": "uint256"
                 }
             ],
-            "name": "getSeriesInfo",
+            "name": "mint",
             "outputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "tuple"
+                    "type": "bool"
+                }
+            ],
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "name",
+            "outputs": [
+                {
+                    "internalType": "string",
+                    "name": "",
+                    "type": "string"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "components": [
-                        {
-                            "internalType": "uint64",
-                            "name": "expiration",
-                            "type": "uint64"
-                        },
-                        {
-                            "internalType": "uint128",
-                            "name": "strike",
-                            "type": "uint128"
-                        },
-                        {
-                            "internalType": "bool",
-                            "name": "isPut",
-                            "type": "bool"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "underlying",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "strikeAsset",
-                            "type": "address"
-                        },
-                        {
-                            "internalType": "address",
-                            "name": "collateral",
-                            "type": "address"
-                        }
-                    ],
-                    "internalType": "struct Types.OptionSeries",
-                    "name": "optionSeries",
-                    "type": "tuple"
+                    "internalType": "address",
+                    "name": "",
+                    "type": "address"
                 }
             ],
-            "name": "issue",
+            "name": "nonces",
             "outputs": [
                 {
-                    "internalType": "address",
+                    "internalType": "uint256",
                     "name": "",
-                    "type": "address"
+                    "type": "uint256"
                 }
             ],
-            "stateMutability": "nonpayable",
+            "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "_series",
+                    "name": "owner",
+                    "type": "address"
+                },
+                {
+                    "internalType": "address",
+                    "name": "spender",
                     "type": "address"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "amount",
+                    "name": "value",
                     "type": "uint256"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "collateralAmount",
+                    "name": "deadline",
                     "type": "uint256"
-                }
-            ],
-            "name": "open",
-            "outputs": [
+                },
                 {
-                    "internalType": "bool",
-                    "name": "",
-                    "type": "bool"
+                    "internalType": "uint8",
+                    "name": "v",
+                    "type": "uint8"
                 },
                 {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
+                    "internalType": "bytes32",
+                    "name": "r",
+                    "type": "bytes32"
+                },
+                {
+                    "internalType": "bytes32",
+                    "name": "s",
+                    "type": "bytes32"
                 }
             ],
+            "name": "permit",
+            "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "address",
-                    "name": "_series",
+                    "internalType": "contract IAuthority",
+                    "name": "_newAuthority",
                     "type": "address"
                 }
             ],
-            "name": "settle",
+            "name": "setAuthority",
+            "outputs": [],
+            "stateMutability": "nonpayable",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "symbol",
             "outputs": [
                 {
-                    "internalType": "bool",
-                    "name": "success",
-                    "type": "bool"
-                },
+                    "internalType": "string",
+                    "name": "",
+                    "type": "string"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [],
+            "name": "totalSupply",
+            "outputs": [
                 {
                     "internalType": "uint256",
-                    "name": "collatReturned",
+                    "name": "",
                     "type": "uint256"
-                },
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "collatLost",
-                    "type": "uint256"
+                    "internalType": "address",
+                    "name": "to",
+                    "type": "address"
                 },
                 {
                     "internalType": "uint256",
-                    "name": "amountShort",
+                    "name": "amount",
                     "type": "uint256"
                 }
             ],
+            "name": "transfer",
+            "outputs": [
+                {
+                    "internalType": "bool",
+                    "name": "",
+                    "type": "bool"
+                }
+            ],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "address",
-                    "name": "series",
+                    "name": "from",
+                    "type": "address"
+                },
+                {
+                    "internalType": "address",
+                    "name": "to",
                     "type": "address"
+                },
+                {
+                    "internalType": "uint256",
+                    "name": "amount",
+                    "type": "uint256"
                 }
             ],
-            "name": "vaultIds",
+            "name": "transferFrom",
             "outputs": [
                 {
-                    "internalType": "uint256",
+                    "internalType": "bool",
                     "name": "",
-                    "type": "uint256"
+                    "type": "bool"
                 }
             ],
-            "stateMutability": "view",
+            "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
-    "bytecode": "0x",
-    "contractName": "IOptionRegistry",
-    "deployedBytecode": "0x",
-    "deployedLinkReferences": {},
-    "linkReferences": {},
-    "sourceName": "contracts/interfaces/IOptionRegistry.sol"
+    "bytecode": "",
+    "deployedBytecode": "",
+    "deployedLinkReferences": "",
+    "sourceName": ""
 }
```

### Comparing `rysk_client-0.2.1/rysk_client/src/collateral.py` & `rysk_client-0.2.2/rysk_client/src/collateral.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from web3 import Web3
 
 
 class Collateral(Enum):
     """Collateral supported by the protocol"""
 
-    WETH = Web3.to_checksum_address("0x3b3a1de07439eeb04492fa64a889ee25a130cdd3")
-    USDC = Web3.to_checksum_address("0x408c5755b5c7a0a28d851558ea3636cfc5b5b19d")
+    WETH = Web3.toChecksumAddress("0x3b3a1de07439eeb04492fa64a889ee25a130cdd3")
+    USDC = Web3.toChecksumAddress("0x408c5755b5c7a0a28d851558ea3636cfc5b5b19d")
 
     @classmethod
     def is_supported(cls, collateral):
         """Is the sset supported"""
         try:
             cls.from_symbol(collateral)
         except ValueError:
```

### Comparing `rysk_client-0.2.1/rysk_client/src/pnl_calculator.py` & `rysk_client-0.2.2/rysk_client/src/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.1/rysk_client/src/position.py` & `rysk_client-0.2.2/rysk_client/src/position.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.1/rysk_client/src/position_manager.py` & `rysk_client-0.2.2/rysk_client/src/position_manager.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.1/rysk_client/src/rysk_option_market.py` & `rysk_client-0.2.2/rysk_client/src/rysk_option_market.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from typing import Dict, List, Optional
 
 from rysk_client.src.collateral import Collateral
-from rysk_client.src.utils import get_contract
 
 HUMAN_NUMBER_FMT = 1e18
 HUMAN_NUMBER_FMT_USDC = 1e6
+EXPIRATION_TIME = "08:00:00"
 
 
 @dataclass
 class TradingSpec:
     """
     Class to represent the trading spec.
     """
@@ -34,14 +34,16 @@
     """
 
     strike: int
     sell: TradingSpec
     buy: TradingSpec
     delta: int
     exposure: int
+    series_collateral_exchange_balance_usdc: Optional[int] = None
+    series_collateral_exchange_balance_weth: Optional[int] = None
 
 
 class OptionChain:
     """Class to represent the option chain."""
 
     _raw_data: tuple
     expirations: List[int]
@@ -79,32 +81,43 @@
             }
 
     def _parse_option_data(self, option_data: tuple):
         """
         Parse the option data.
         """
         markets = []
-        for (
-            strike,
-            sell_trading_specs,
-            buy_trading_specs,
-            delta,
-            net_dhv_exposure,
-        ) in option_data:
-            sell_trading_specs = TradingSpec(*sell_trading_specs)
-            buy_trading_specs = TradingSpec(*buy_trading_specs)
-            markets.append(
-                OptionStrikeDrill(
-                    strike,
-                    sell_trading_specs,
-                    buy_trading_specs,
-                    delta,
-                    net_dhv_exposure,
-                )
-            )
+        if len(option_data[0]) == 5:
+            cols = [
+                "strike",
+                "sell_trading_specs",
+                "buy_trading_specs",
+                "delta",
+                "exposure",
+            ]
+        elif len(option_data[0]) == 7:
+            cols = [
+                "strike",
+                "sell_trading_specs",
+                "buy_trading_specs",
+                "delta",
+                "exposure",
+                "series_collateral_exchange_balance_usdc",
+                "series_collateral_exchange_balance_weth",
+            ]
+        else:
+            raise ValueError("Option data has unexpected length. is not beta or prod.")
+
+        for row in option_data:
+            params = {}
+            for k, val in zip(cols, row):
+                if k in ["sell_trading_specs", "buy_trading_specs"]:
+                    params[k.split("_")[0]] = TradingSpec(*val)
+                else:
+                    params[k] = val
+            markets.append(OptionStrikeDrill(**params))
         return markets
 
     @property
     def active_markets(self):
         """Return the active strikes for the active markets, where option drill is not disabled."""
         active_markets = []
         for expiration, option_drill in self.strikes.items():
@@ -129,25 +142,27 @@
     """Option type enum."""
 
     CALL = "call"
     PUT = "put"
 
 
 @dataclass
-class RyskOptionMarket:
+class RyskOptionMarket:  # pylint: disable=too-many-instance-attributes
     """Rysk option market."""
 
     strike: float
     expiration: int
     is_put: bool
     active: bool = True
     # market data
     bid: Optional[int] = None
     ask: Optional[int] = None
     dhv: Optional[int] = None
+    delta: Optional[int] = None
+    _collateral: Optional[Collateral] = None
 
     @classmethod
     def from_series(cls, series):
         """Returns a RyskOptionMarket from a series"""
         return cls(
             strike=series["strike"],
             expiration=series["expiration"],
@@ -180,80 +195,69 @@
         return cls(
             strike=option_drill.strike,
             expiration=expiration,
             is_put=option_type == "put",
             ask=option_drill.buy.quote,
             bid=option_drill.sell.quote,
             dhv=option_drill.exposure,
+            delta=option_drill.delta,
         )
 
     def to_json(self):
         """Returns the option market as a json"""
         market_data = {}
-        if self.bid and self.ask and self.dhv:
+        if self.bid and self.ask and self.dhv is not None:
             market_data = {
                 "bid": self.bid / HUMAN_NUMBER_FMT_USDC,
                 "ask": self.ask / HUMAN_NUMBER_FMT_USDC,
                 "dhv": self.dhv / HUMAN_NUMBER_FMT,
             }
         result = {
             "id": self.name,
             "strike": self.strike / HUMAN_NUMBER_FMT,
             "expiration": self.expiration,
             "optionType": "put" if self.is_put else "call",
             "active": self.active,
         }
+        if self.delta:
+            result["delta"] = self.delta / HUMAN_NUMBER_FMT
         result.update(**market_data)
         return result
 
     def to_series(self):
         """
         creates a json series object compatible with the rysk contracts.
         """
         return {
             "strike": self.strike,
             "expiration": self.expiration,
             "isPut": self.is_put,
             "underlying": Collateral.WETH.value,
             "strikeAsset": Collateral.USDC.value,
-            "collateral": Collateral.USDC.value
-            if self.is_put
-            else Collateral.WETH.value,
+            "collateral": self.collateral.value,
         }
 
+    @classmethod
+    def from_str(cls, name: str):
+        """Returns a RyskOptionMarket from a name"""
+        _name = name.split("-")
+        expiration_date = datetime.strptime(
+            f"{_name[1]}T{EXPIRATION_TIME}+00:00",
+            "%d%b%yT%H:%M:%S%z",
+        )
+        _expiration = int(expiration_date.timestamp())
 
-class RyskOptionMarketManager:
-    """Class to represent the RyskOptionMarketManager."""
-
-    def fetch_option_markets(self):
-        """Fetches the option markets from the API"""
-        markets = []
-        for expiration in self._fetch_expirations():
-            put_strikes = self.option_catalogue.functions.getOptionDetails(
-                expiration, True
-            ).call()
-            call_strikes = self.option_catalogue.functions.getOptionDetails(
-                expiration, False
-            ).call()
-
-            for strike in put_strikes:
-                markets.append(RyskOptionMarket(expiration, strike, True))
-
-            for strike in call_strikes:
-                markets.append(RyskOptionMarket(expiration, strike, False))
-        self.option_markets = markets
-        return markets
-
-    def __init__(self, web3):
-        self.web3 = web3
-        self.option_markets = {}
-        self.option_catalogue = get_contract("option_catalogue", web3)
-        self.fetch_option_markets()
-
-    def fetch_option_market(self, name):
-        """
-        Fetches a specific option market from the smart contract.
-        """
+        _strike = int(_name[2]) * 10**18
+        _is_put = _name[3] == "P"
+        return cls(_strike, _expiration, _is_put)
 
-    def _fetch_expirations(self):
-        """Returns the expirations from the smart contract."""
-        return self.option_catalogue.functions.getExpirations().call()
+    @property
+    def collateral(self):
+        """Returns the collateral of the option market"""
+        if self._collateral is None:
+            return Collateral.USDC if self.is_put else Collateral.WETH
+        return self._collateral
+
+    @collateral.setter
+    def collateral(self, collateral):
+        """Sets the collateral of the option market"""
+        self._collateral = collateral
```

### Comparing `rysk_client-0.2.1/rysk_client/src/subgraph.py` & `rysk_client-0.2.2/rysk_client/src/subgraph.py`

 * *Files 17% similar despite different names*

```diff
@@ -129,16 +129,19 @@
         subgraph_query = {"query": query}
         response = requests.post(
             url=self.url,
             headers=headers,
             data=json.dumps(subgraph_query),
             timeout=DEFAULT_TIMEOUT,
         )
-        data = json.loads(response.content)["data"]
-        return data
+        if response.status_code != 200 or response.content == b"404":
+            raise ValueError(
+                f"Subgraph query failed with status code {response.status_code}."
+            )
+        return json.loads(response.content)["data"]
 
     def query_markets(self):
         """Query the subgraph for markets."""
         return self._query(MARKET_SUBGRAPH_QUERY)["series"]
 
     def query_longs(self, address: str) -> List[Dict[str, Any]]:
         """Query the subgraph for longs."""
```

### Comparing `rysk_client-0.2.1/rysk_client/src/utils.py` & `rysk_client-0.2.2/rysk_client/src/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 """
 Helper functions for the rysk_client package.
 """
 import json
 import logging
-import os
-from copy import deepcopy
+import sys
+from dataclasses import asdict
 from typing import List, Optional
 
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.table import Table
 from web3 import Web3
 
-from rysk_client.src.constants import ADDRESSES, DEFAULT_ENCODING, RPC_URL
+from rysk_client.src.constants import (ARBITRUM_GOERLI, DEFAULT_ENCODING,
+                                       PROTOCOL_DEPLOYMENTS)
 
 
 def get_logger():
     """Get the logger."""
     logger = logging.getLogger(__name__)
     formatter = logging.Formatter("%(message)s")
 
-    handler = RichHandler(
-        markup=False,
-        rich_tracebacks=True,
-        locals_max_string=None,
-        locals_max_length=None,
-    )
+    # we check if the logger already has a handler
+    # to avoid adding multiple handlers
+    if logger.hasHandlers():
+        return logger
+    if sys.stdout.isatty():
+
+        handler = RichHandler(
+            markup=False,
+            rich_tracebacks=True,
+            locals_max_string=None,
+            locals_max_length=None,
+        )
+    else:
+        handler = logging.StreamHandler(sys.stdout)
 
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
     return logger
 
 
-def get_contract(name, web3):
+def get_contract(name, web3, chain, address=None):
     """Returns a web3 contract instance for the given contract name"""
-    path = os.path.join(os.path.dirname(__file__), "..")
-    spec = ADDRESSES[name]
-    with open(f"{path}/{spec['path']}", "r", encoding=DEFAULT_ENCODING) as abi:
+    spec = PROTOCOL_DEPLOYMENTS[chain.name].contracts[name]
+
+    with open(spec.path, "r", encoding=DEFAULT_ENCODING) as abi:
         abi = json.loads(abi.read())["abi"]
-    res = deepcopy(spec)
+    res = asdict(spec)
     del res["path"]
     res["abi"] = abi
+    if address is not None:
+        res["address"] = address
     return web3.eth.contract(**res)
 
 
-def get_web3(rpc_url: Optional[str] = None) -> Web3:
+def get_web3(chain=ARBITRUM_GOERLI) -> Web3:
     """Returns a web3 instance connected to RPC_URL"""
-    if rpc_url is None:
-        rpc_url = RPC_URL
-    web3 = Web3(Web3.HTTPProvider(rpc_url))
+
+    web3 = Web3(Web3.HTTPProvider(chain.rpc_url))
     return web3
 
 
 def render_table(title: str, data, cols: Optional[List[str]] = None):
     """Render a table from a dynamic input."""
     table = Table(title=title)
     # we first create the columns
```

### Comparing `rysk_client-0.2.1/rysk_client/web3_client.py` & `rysk_client-0.2.2/rysk_client/web3_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,66 @@
 """
 Web3 client for RyskFinance.
 """
 import json
 import logging
 from collections import deque
+from copy import deepcopy
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple
 
 import websocket
+from rich import print_json
+from web3 import HTTPProvider
 from web3.contract import Contract
 
 from rysk_client.src.action_type import ActionType
 from rysk_client.src.collateral import Collateral
-from rysk_client.src.constants import NULL_ADDRESS, RPC_URL, WSS_URL
+from rysk_client.src.constants import (ARBITRUM_GOERLI, NULL_ADDRESS,
+                                       NULL_DATA, Chain)
 from rysk_client.src.crypto import EthCrypto
+from rysk_client.src.operation_factory import close_long, close_short
 from rysk_client.src.order import Order
 from rysk_client.src.order_side import OrderSide
 from rysk_client.src.utils import get_contract, get_logger, get_web3
 
 
+def print_operate_tuple(operate_tuple: List[Dict[str, Any]]):
+    """
+    Ensure that the operate tuple is formated ina manner compatible with
+    tenderly's api.
+    print it using rich.
+    """
+    display_tuple = deepcopy(operate_tuple)
+    keys_to_stringify = [
+        "strike",
+        "amount",
+        "indexOrAcceptablePremium",
+        "vaultId",
+        "actionType",
+    ]
+
+    def stringify_json(json_data: Any):
+        """
+        Recursively stringify json data.
+        """
+        if isinstance(json_data, dict):
+            for key, value in json_data.items():
+                if key in keys_to_stringify:
+                    json_data[key] = str(value)
+                else:
+                    stringify_json(value)
+        elif isinstance(json_data, list):
+            for value in json_data:
+                stringify_json(value)
+
+    stringify_json(display_tuple)
+    print_json(data=display_tuple)
+
+
 class Balances(Enum):
     """
     Class to represent the balances of an address.
     """
 
 
 class Web3Client:  # pylint: disable=too-many-instance-attributes
@@ -41,37 +79,52 @@
     usdc: Contract
     weth: Contract
 
     def __init__(
         self,
         logger: Optional[logging.Logger] = None,
         crypto: Optional[EthCrypto] = None,
-        rpc_url: str = RPC_URL,
+        chain: Chain = ARBITRUM_GOERLI,
+        verbose: bool = True,
     ):
         """
         Initialize the client with the web3 provider.
         """
-        self.web3 = get_web3(rpc_url)
-        self.beyond_pricer = get_contract("beyond_pricer", self.web3)
-        self.opyn_controller = get_contract("opyn_controller", self.web3)
-        self.option_exchange = get_contract("option_exchange", self.web3)
-        self.option_registry = get_contract("option_registry", self.web3)
+        self.chain = chain
+        self.web3: HTTPProvider = get_web3(chain)
+        self.beyond_pricer = get_contract("beyond_pricer", self.web3, self.chain)
+        self.opyn_controller = get_contract("opyn_controller", self.web3, self.chain)
+        self.option_exchange = get_contract("option_exchange", self.web3, self.chain)
+        self.option_registry = get_contract(
+            "opyn_option_registry", self.web3, self.chain
+        )
 
-        self.user_position_lens_mk1 = get_contract("user_position_lens_mk1", self.web3)
-        self.dhv_lens_mk1 = get_contract("dhv_lens_mk1", self.web3)
+        self.user_position_lens_mk1 = get_contract(
+            "user_position_lens", self.web3, self.chain
+        )
+        self.dhv_lens_mk1 = get_contract("d_h_v_lens", self.web3, self.chain)
 
-        self.usdc = get_contract("usdc", self.web3)
-        self.weth = get_contract("weth", self.web3)
+        self.usdc = get_contract("usdc", self.web3, self.chain)
+        self.weth = get_contract("weth", self.web3, self.chain)
         # is this an artifact of the testnet?
-        self.settlement_usdc = get_contract("settlement_usdc", self.web3)
-        self.settlement_weth = get_contract("settlement_weth", self.web3)
+        self.settlement_usdc = get_contract("usdc", self.web3, self.chain)
+        self.settlement_weth = get_contract("weth", self.web3, self.chain)
 
         self._logger = logger or get_logger()
         self._processed_tx: deque = deque(maxlen=100)
         self._crypto = crypto
+        self._verbose = verbose
+
+    def get_otoken_contract(self, otoken_address: str) -> Contract:
+        """
+        Get the otoken contract.
+        """
+        return get_contract(
+            "o_token", self.web3, chain=self.chain, address=otoken_address
+        )
 
     def get_options_prices(
         self,
         option_data,
         dhv_exposure,
         amount=1000000000000000000,
         side="buy",
@@ -107,34 +160,34 @@
             ).call()
         except Exception as error:  # pylint: disable=broad-except
             self._logger.error(
                 f"Error calling beyond pricer: {error} with {option_series}"
             )
 
             return 0
-        return result[0] / 1_000_000
+        return result[0]
 
     def get_balances(self):
         """
         Get the balances for an address
         """
-        safe_address = self.web3.to_checksum_address(self._crypto.address)
+        safe_address = self.web3.toChecksumAddress(self._crypto.address)
         return {
             "weth": self.settlement_weth.functions.balanceOf(safe_address).call()
             / 1e18,
             "usdc": self.settlement_usdc.functions.balanceOf(safe_address).call() / 1e6,
             "eth": self.web3.eth.get_balance(self._crypto.address) / 1e18,
         }
 
     def watch_trades(self):
         """
         Subscribe to boeht pending trades and completed trades.
         """
         ws_connection = websocket.WebSocketApp(
-            WSS_URL,
+            self.chain.wss_url,
             on_open=self.on_open,
             on_message=self.on_message,
             on_error=self.on_error,
             on_close=self.on_close,
         )
         ws_connection.run_forever()
 
@@ -196,62 +249,51 @@
             rich_logs = self.option_exchange.events.OptionsSold().processReceipt(tx_receipt)  # type: ignore
             return dict(rich_logs[0]["args"]), False
 
         except Exception:  # pylint: disable=W0718
             rich_logs = self.option_exchange.events.OptionsBought().processReceipt(tx_receipt)  # type: ignore
             return dict(rich_logs[0]["args"]), False
 
-        except Exception as exc:  # pylint: disable=W0718,W0705
-            self._logger.error(
-                f"An exception occurred while trying to get the transaction arguments for {tx_receipt}: {exc}"
-            )
-            return {}, True
-
-    def sign_and_sumbit(self, txn: dict, private_key: str) -> str:  # type: ignore
-        """
-        Sign the transaction with the private key and send it to the blockchain.
-        """
-
-        signed_txn = self.web3.eth.account.sign_transaction(
-            txn, private_key=private_key
-        )
-        tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-        self._logger.debug(f"Transaction hash: {tx_hash.hex()}")
-        receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, 180)
-        # we need to check the receipt to see if the transaction was successful
-        if receipt["status"] == 0:
-            self._logger.error(f"Transaction failed: {receipt}")
-            return False  # type: ignore
-        self._logger.debug(f"Transaction successful: {receipt}")
-        return tx_hash.hex()
-
     def is_approved(
         self, contract: Contract, spender: str, owner: str, amount: int
     ) -> bool:
         """
         Check if the spender is approved to spend the owner's tokens.
         """
-        return contract.functions.allowance(owner, spender).call() >= amount
+        allowance = contract.functions.allowance(owner, spender).call()
+        return allowance >= amount
 
     def create_approval(
         self, contract: Contract, spender: str, owner: str, amount: int
     ) -> dict:
         """
         Create an approval transaction.
         """
         transaction = contract.functions.approve(
             spender, int(amount)
         ).build_transaction(
             {
-                "from": owner,
-                "nonce": self.web3.eth.get_transaction_count(owner),
+                **{
+                    "from": owner,
+                    "nonce": self.web3.eth.get_transaction_count(owner),
+                },
+                **self._default_tx_params,
             }
         )
         return transaction
 
+    @property
+    def _default_tx_params(self) -> dict:
+        """
+        Default transaction parameters.
+        """
+        return {
+            "gasPrice": int(self.web3.eth.gas_price * 1.5),
+        }
+
     def fetch_user_vaults(self, address: str) -> List[Dict[str, Any]]:  # noqa: W0613
         """
         Fetch the user's positions from the options exchange.
         """
         return self.user_position_lens_mk1.functions.getVaultsForUser(
             str(self._crypto.address)  # type: ignore
         ).call()
@@ -274,15 +316,15 @@
         """
         arguments = (
             Collateral.WETH.value,
             Collateral.USDC.value,
             series["expiration"],
             series["isPut"],
             series["strike"],
-            Collateral.USDC.value if series["isPut"] else Collateral.WETH.value,
+            series["collateral"],
         )
         return self.option_registry.functions.getOtoken(*arguments).call()
 
     def settle_vault(self, vault_id: int):
         """Build the transaction to settle the vault."""
         operate_tuple = [
             {
@@ -294,11 +336,125 @@
                 "owner": self._crypto.address,  # type: ignore
                 "secondAddress": self._crypto.address,  # type: ignore
                 "vaultId": vault_id,
             },
         ]
         return self.opyn_controller.functions.operate(operate_tuple).build_transaction(
             {
-                "from": self._crypto.address,  # type: ignore
-                "nonce": self.web3.eth.get_transaction_count(self._crypto.address),  # type: ignore
+                **{
+                    "from": self._crypto.address,  # type: ignore
+                    "nonce": self.web3.eth.get_transaction_count(self._crypto.address),  # type: ignore
+                },
+                **self._default_tx_params,
+            }
+        )
+
+    def redeem_otoken(
+        self,
+        otoken_id: str,
+        amount: int,
+    ):
+        """
+        Build the transaction to redeem the otoken.
+        """
+        self._logger.info(
+            f"Redeeming {amount} of {self.web3.toChecksumAddress(otoken_id)}"
+        )
+        amount = int(amount * 1e8)
+        operate_tuple = [
+            {
+                "actionType": 8,
+                "owner": NULL_ADDRESS,
+                "secondAddress": self._crypto.address,  # type: ignore
+                "asset": otoken_id,
+                "vaultId": 0,
+                "amount": amount,
+                "index": 0,
+                "data": NULL_DATA,
+            }
+        ]
+        return self.opyn_controller.functions.operate(operate_tuple).build_transaction(
+            {
+                **{
+                    "from": self._crypto.address,  # type: ignore
+                    "nonce": self.web3.eth.get_transaction_count(self._crypto.address),  # type: ignore
+                },
+                **self._default_tx_params,
+            }
+        )
+
+    def get_otoken_balance(self, otoken_id: str):
+        """
+        Get the otoken balance.
+        """
+        otoken = get_contract("o_token", self.web3, chain=self.chain, address=otoken_id)
+        return otoken.functions.balanceOf(self._crypto.address).call()  # type: ignore
+
+    def close_long(
+        self,
+        acceptable_premium: int,
+        amount: int,
+        otoken_address: str,
+    ):
+        """
+        Build the transaction to close a long position.
+        """
+        operate_tuple = close_long(
+            acceptable_premium=acceptable_premium,
+            owner_address=self._crypto.address,  # type: ignore
+            otoken_address=otoken_address,
+            amount=int(amount),
+        )
+        if self._verbose:
+            print_operate_tuple(operate_tuple)
+
+        return self.option_exchange.functions.operate(operate_tuple).build_transaction(
+            {
+                **{
+                    "from": self._crypto.address,  # type: ignore
+                    "nonce": self.web3.eth.get_transaction_count(self._crypto.address),  # type: ignore
+                },
+                **self._default_tx_params,
+            }
+        )
+
+    def get_series_info(self, otoken_address: str) -> Dict[str, Any]:
+        """
+        Returns the series info.
+        """
+        return self.option_registry.functions.getSeriesInfo(otoken_address).call()
+
+    def close_short(
+        self,
+        acceptable_premium: int,
+        amount: int,
+        otoken_address: str,
+        collateral_amount: int,
+        collateral_asset: str,
+        vault_id: int,
+        rysk_option_market: str,
+    ):
+        """
+        Build the transaction to close a short position.
+        """
+        operate_tuple = close_short(
+            acceptable_premium=acceptable_premium,
+            owner_address=self._crypto.address,  # type: ignore
+            otoken_address=self.web3.toChecksumAddress(otoken_address),
+            amount=int(amount),
+            collateral_amount=int(collateral_amount),
+            collateral_asset=collateral_asset.value,
+            vault_id=vault_id,
+            rysk_option_market=rysk_option_market,
+        )
+        if self._verbose:
+            print_operate_tuple(operate_tuple)
+
+        return self.option_exchange.functions.operate(operate_tuple).build_transaction(
+            {
+                **{
+                    "from": self._crypto.address,  # type: ignore
+                    "nonce": self.web3.eth.get_transaction_count(self._crypto.address),  # type: ignore
+                },
+                **self._default_tx_params,
             }
         )
```

### Comparing `rysk_client-0.2.1/PKG-INFO` & `rysk_client-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: rysk-client
-Version: 0.2.1
-Summary: 
-Author: 8baller
-Author-email: 8ball030@gmail.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ccxt (>=3.1.15,<4.0.0)
-Requires-Dist: rich-click (>=1.6.1,<2.0.0)
-Requires-Dist: web3 (==6.4.0)
-Requires-Dist: websocket-client (>=1.6.1,<2.0.0)
-Description-Content-Type: text/markdown
-
 # Rysk Client
 
 ## Installation
 
 The application is availale on pypi and can be installed as so;
 
     ```bash
@@ -200,14 +182,18 @@
     │ ETH-30JUN… │ short │ 0          │ 0x9b8a20… │ 0.0   │ 0.0        │ 21249.08… │
     │ ETH-30JUN… │ short │ 105.35629… │ 0x9b8a20… │ -2.0  │ 210.712583 │ 0         │
     │ ETH-30JUN… │ short │ 118.16245… │ 0x9b8a20… │ -14.0 │ 1654.2744… │ 0         │
     │ ETH-30JUN… │ short │ 106.420235 │ 0x9b8a20… │ -1.0  │ 106.420235 │ 0         │
     └────────────┴───────┴────────────┴───────────┴───────┴────────────┴───────────┘
 
 
+## Expired positions
+
+We can use the `--expired` flag in order to filter for the expired positions
+
 
 ```python
 ! export ETH_ADDRESS=0x9B8a204636a7aa9c33053d9C3A828720d32212e8 && \
   export ETH_PRIVATE_KEY=0x75cc9212e9e1243b9a3e5db5012f39469254088e33363324ad94dd0b212d7efa && \
     rysk positions list --expired
 ```
 
@@ -240,19 +226,54 @@
     │ ETH-16JU… │ short │ 21.762156… │ 0x9b8a20… │ -20.0  │ 435.24313… │ 0         │
     │ ETH-26MA… │ short │ 50.9876923 │ 0x9b8a20… │ -10.0  │ 509.876923 │ 0         │
     │ ETH-02JU… │ short │ 31.792668  │ 0x9b8a20… │ -1.0   │ 31.792668  │ 0         │
     │ ETH-26MA… │ short │ 47.281672… │ 0x9b8a20… │ -40.0  │ 1891.2668… │ 0         │
     └───────────┴───────┴────────────┴───────────┴────────┴────────────┴───────────┘
 
 
+## Settling Positions
+We are able to settle the positions based on the vault id
+
 
 ```python
 
+! export ETH_ADDRESS=0x9B8a204636a7aa9c33053d9C3A828720d32212e8 && \
+  export ETH_PRIVATE_KEY=0x75cc9212e9e1243b9a3e5db5012f39469254088e33363324ad94dd0b212d7efa && \
+  rysk positions settle -v 15
 ```
 
+    [2;36m[06/23/23 01:02:47][0m[2;36m [0m[34mINFO    [0m Settling vault [1;36m15[0m for                    ]8;id=770874;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/cli.py\[2mcli.py[0m]8;;\[2m:[0m]8;id=837991;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/cli.py#148\[2m148[0m]8;;\
+    [2;36m                    [0m         [1;36m0x9B8a204636a7aa9c33053d9C3A828720d32212[0m [2m          [0m
+    [2;36m                    [0m         [1;36me8[0m                                       [2m          [0m
+    [2;36m                   [0m[2;36m [0m[34mINFO    [0m Rysk client initialized and connected  ]8;id=936728;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/client.py\[2mclient.py[0m]8;;\[2m:[0m]8;id=522814;file:///home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/client.py#99\[2m99[0m]8;;\
+    [2;36m                    [0m         to the blockchain at RPC connection    [2m            [0m
+    [2;36m                    [0m         [4;94mhttps://arbitrum-goerli.rpc.thirdweb.c[0m [2m            [0m
+    [2;36m                    [0m         [4;94mom[0m                                     [2m            [0m
+    Traceback (most recent call last):
+      File "/home/tom/.pyenv/versions/3.10.4/bin/rysk", line 8, in <module>
+        sys.exit(cli())
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1126, in __call__
+        return self.main(*args, **kwargs)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rich_click/rich_group.py", line 21, in main
+        rv = super().main(*args, standalone_mode=False, **kwargs)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1051, in main
+        rv = self.invoke(ctx)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1657, in invoke
+        return _process_result(sub_ctx.command.invoke(sub_ctx))
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1657, in invoke
+        return _process_result(sub_ctx.command.invoke(sub_ctx))
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 1393, in invoke
+        return ctx.invoke(self.callback, **ctx.params)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/click/core.py", line 752, in invoke
+        return __callback(*args, **kwargs)
+      File "/home/tom/.pyenv/versions/3.10.4/lib/python3.10/site-packages/rysk_client/cli.py", line 158, in settle
+        raise ValueError(
+    ValueError: Vault 15 has already been settled for 0x9B8a204636a7aa9c33053d9C3A828720d32212e8
+
+
 ## Creating a Client 
 
 Clients can be created from the rysk client module.
 
 
 ```python
 from rysk_client.client import RyskClient
@@ -590,7 +611,22 @@
     [34m19 files [0mleft unchanged.
     poetry run adev lint -v -p tests
     [2;36m[14:13:44][0m[2;36m [0m[34mINFO    [0m Linting Open Autonomy Packages                     ]8;id=281004;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py\[2mcli.py[0m]8;;\[2m:[0m]8;id=265993;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py#47\[2m47[0m]8;;\
     [2KLinting... [38;2;114;156;31m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [35m100%[0m [33m0:00:03[0m
     [?25h[2;36m[14:13:48][0m[2;36m [0m[34mINFO    [0m Linting completed successfully!                    ]8;id=864081;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py\[2mcli.py[0m]8;;\[2m:[0m]8;id=992553;file:///home/tom/.cache/pypoetry/virtualenvs/rysk-client-O72xupT4-py3.10/lib/python3.10/site-packages/auto_dev/cli.py#66\[2m66[0m]8;;\
 
 
+
+```python
+
+```
+
+# Releasing
+Git ops is used to enable automated releases via pypi.
+
+```bash
+export NEW_VERSION=0.2.0
+git checkout -b v$NEW_VERSION
+bumpversion  rysk_client/ --new-version $NEW_VERSION
+git push && git push --tag
+
+```
```

