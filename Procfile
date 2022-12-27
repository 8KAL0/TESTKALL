# Add command handlers
    dp.add_handler(CommandHandler("start", start))
    dp.add_handler(CommandHandler("products", product))
    dp.add_handler(CommandHandler("add", add_to_cart))
    dp.add_handler(CommandHandler("remove", remove_from_cart))
    dp.add_handler(CommandHandler("cart", show_cart))
    dp.add_handler(CommandHandler("checkout", checkout))

    # Add callback query handler
    dp.add_handler(CallbackQueryHandler(pay))

    # log all errors
    dp.add_error_handler(error)

    # Start the Bot
    updater.start_polling()

    # Run the bot until you press Ctrl-C or the process receives SIGINT,
    # SIGTERM or SIGABRT. This should be used most of the time, since
    # start_polling() is non-blocking and will stop the bot gracefully.
    updater.idle()

if name == '__main__':
    main()
