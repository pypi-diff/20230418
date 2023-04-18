# Comparing `tmp/telebox-0.9.1.tar.gz` & `tmp/telebox-0.9.2.tar.gz`

## Comparing `telebox-0.9.1.tar` & `telebox-0.9.2.tar`

### file list

```diff
@@ -1,257 +1,257 @@
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/errors.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/context/__init__.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/context/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/context/state_machine.py
--rw-r--r--   0        0        0    54855 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/context/telegram_bot.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/context/utils.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/context/vars.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/__init__.py
--rw-r--r--   0        0        0    25477 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/dispatcher.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/errors.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/typing.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/enums/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/enums/event_type.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/enums/media_group_content_type.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/__init__.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/error_filter.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event_filter.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/error/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/error/none.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/error/reg_exp_text.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/error/text.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/error/type.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/__init__.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/callback_data.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/cashtag.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/chat_id.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/chat_type.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/command.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/forwarded_message.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/hashtag.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/media_group_content_type.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/mention.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/message_content_type.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/non_standard_command.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/none.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/reg_exp_text.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/reply_message.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/sender_contact.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/simple_callback_data.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/state.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/text.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/text_mention.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/filters/event/user_id.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/handlers/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/handlers/error.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/handlers/event.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/middlewares/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/middlewares/middleware.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/middlewares/middlewares/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/middlewares/middlewares/callback_data.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/__init__.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/event_queue.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/events.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/media_group.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/server_root.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/timed_container.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/__init__.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/call_tracker.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/rate_limit.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/rate_limiter.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/errors.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/machine.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/magazine.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/manager.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/state.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/transition_scheme.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/storages/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/storages/storage.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/storages/storages/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/storages/storages/file.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/state_machine/storages/storages/memory.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/__init__.py
--rw-r--r--   0        0        0    24818 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/errors.py
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/serializer.py
--rw-r--r--   0        0        0    82801 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/telegram_bot.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/bot_command_scope_types.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/chat_actions.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/chat_member_statuses.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/chat_types.py
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/country_codes.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/currencies.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/dice_emojis.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/encrypted_passport_element_types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/inline_query_chat_types.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/inline_query_result_types.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/input_media_types.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/language_codes.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/mask_position_points.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/menu_button_types.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/message_entity_types.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/parse_modes.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/passport_element_error_sources.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/poll_types.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/sticker_types.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/consts/update_types.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/enums/__init__.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/enums/message_content_type.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/enums/update_content_type.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/type.py
--rw-r--r--   0        0        0    10271 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/animation.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/audio.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_chat.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope_default.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/callback_game.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/callback_query.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_administrator_rights.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_invite_link.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_join_request.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_location.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_administrator.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_banned.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_left.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_member.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_owner.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_restricted.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_updated.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_permissions.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chat_photo.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/chosen_inline_result.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/contact.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/dice.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/document.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/encrypted_credentials.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/encrypted_passport_element.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/file.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/force_reply.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/game.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/game_high_score.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_keyboard_button.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_keyboard_markup.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_article.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_audio.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_document.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_gif.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_mpeg4_gif.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_video.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_contact.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_document.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_game.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_gif.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_location.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_mpeg4_gif.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_photo.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_venue.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_video.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_voice.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_contact_message_content.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_file.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_invoice_message_content.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_location_message_content.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_media.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_media_animation.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_media_audio.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_media_document.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_media_photo.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_media_video.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_message_content.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_text_message_content.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/input_venue_message_content.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/invoice.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/keyboard_button.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/keyboard_button_poll_type.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/labeled_price.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/location.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/login_url.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/mask_position.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/menu_button.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/menu_button_commands.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/menu_button_default.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/menu_button_web_app.py
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/message.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/message_auto_delete_timer_changed.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/message_entity.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/message_id.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/order_info.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_data.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_data_field.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_file.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_files.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_front_side.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_reverse_side.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_selfie.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_translation_file.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_translation_files.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error_unspecified.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/passport_file.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/photo_size.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/poll.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/poll_answer.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/poll_option.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/pre_checkout_query.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/proximity_alert_triggered.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/reply_keyboard_markup.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/reply_keyboard_remove.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/response_parameters.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/sent_web_app_message.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/shipping_address.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/shipping_option.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/shipping_query.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/sticker.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/sticker_set.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/successful_payment.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/update.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/user.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/user_profile_photos.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/venue.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/video.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/video_chat_ended.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/video_chat_participants_invited.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/video_chat_scheduled.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/video_chat_started.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/video_note.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/voice.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/web_app_data.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/web_app_info.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/telegram_bot/types/types/webhook_info.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/named_set.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/not_set.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/task_executor.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/thread_pool.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/callback_data_builders/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/callback_data_builders/builder.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/callback_data_builders/builders/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/callback_data_builders/builders/json.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/callback_data_builders/builders/separatory.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/env/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/env/env.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 telebox-0.9.1/telebox/utils/env/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telebox-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 telebox-0.9.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 telebox-0.9.1/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 telebox-0.9.1/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 telebox-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 telebox-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/errors.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/context/__init__.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/context/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/context/state_machine.py
+-rw-r--r--   0        0        0    54855 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/context/telegram_bot.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/context/utils.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/context/vars.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/__init__.py
+-rw-r--r--   0        0        0    25477 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/dispatcher.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/errors.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/typing.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/enums/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/enums/event_type.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/enums/media_group_content_type.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/__init__.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/error_filter.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event_filter.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/error/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/error/none.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/error/reg_exp_text.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/error/text.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/error/type.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/callback_data.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/cashtag.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/chat_id.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/chat_type.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/command.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/forwarded_message.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/hashtag.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/media_group_content_type.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/mention.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/message_content_type.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/non_standard_command.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/none.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/reg_exp_text.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/reply_message.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/sender_contact.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/simple_callback_data.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/state.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/text.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/text_mention.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/filters/event/user_id.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/handlers/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/handlers/error.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/handlers/event.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/middlewares/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/middlewares/middleware.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/middlewares/middlewares/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/middlewares/middlewares/callback_data.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/event_queue.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/events.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/media_group.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/server_root.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/timed_container.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/__init__.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/call_tracker.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/rate_limit.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/rate_limiter.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/errors.py
+-rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/machine.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/magazine.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/manager.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/state.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/transition_scheme.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/storages/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/storages/storage.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/storages/storages/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/storages/storages/file.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/state_machine/storages/storages/memory.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/__init__.py
+-rw-r--r--   0        0        0    24818 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/errors.py
+-rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/serializer.py
+-rw-r--r--   0        0        0    82801 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/telegram_bot.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/bot_command_scope_types.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/chat_actions.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/chat_member_statuses.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/chat_types.py
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/country_codes.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/currencies.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/dice_emojis.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/encrypted_passport_element_types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/inline_query_chat_types.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/inline_query_result_types.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/input_media_types.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/language_codes.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/mask_position_points.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/menu_button_types.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/message_entity_types.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/parse_modes.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/passport_element_error_sources.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/poll_types.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/sticker_types.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/consts/update_types.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/enums/__init__.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/enums/message_content_type.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/enums/update_content_type.py
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/type.py
+-rw-r--r--   0        0        0    10271 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/animation.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/audio.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_chat.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope_default.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/callback_game.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/callback_query.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_administrator_rights.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_invite_link.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_join_request.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_location.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_administrator.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_banned.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_left.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_member.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_owner.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_restricted.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_updated.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_permissions.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chat_photo.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/chosen_inline_result.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/contact.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/dice.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/document.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/encrypted_credentials.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/encrypted_passport_element.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/file.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/force_reply.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/game.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/game_high_score.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_keyboard_button.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_keyboard_markup.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_article.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_audio.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_gif.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_mpeg4_gif.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_contact.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_document.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_game.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_gif.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_location.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_mpeg4_gif.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_photo.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_venue.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_video.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_voice.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_contact_message_content.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_file.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_invoice_message_content.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_location_message_content.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_media.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_media_animation.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_media_audio.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_media_document.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_media_photo.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_media_video.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_message_content.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_text_message_content.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/input_venue_message_content.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/invoice.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/keyboard_button.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/labeled_price.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/location.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/login_url.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/mask_position.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/menu_button.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/menu_button_commands.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/menu_button_default.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/menu_button_web_app.py
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/message.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/message_auto_delete_timer_changed.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/message_entity.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/message_id.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/order_info.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_data.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_data_field.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_file.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_files.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_front_side.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_reverse_side.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_selfie.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_translation_file.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_translation_files.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error_unspecified.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/passport_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/photo_size.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/poll.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/poll_answer.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/poll_option.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/pre_checkout_query.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/proximity_alert_triggered.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/reply_keyboard_markup.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/reply_keyboard_remove.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/response_parameters.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/sent_web_app_message.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/shipping_address.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/shipping_option.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/shipping_query.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/sticker.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/sticker_set.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/successful_payment.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/update.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/user.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/user_profile_photos.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/venue.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/video.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/video_chat_ended.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/video_chat_participants_invited.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/video_chat_scheduled.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/video_chat_started.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/video_note.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/voice.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/web_app_data.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/web_app_info.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/telegram_bot/types/types/webhook_info.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/named_set.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/not_set.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/task_executor.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/thread_pool.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/callback_data_builders/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/callback_data_builders/builder.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/callback_data_builders/builders/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/callback_data_builders/builders/json.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/callback_data_builders/builders/separatory.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/env/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/env/env.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 telebox-0.9.2/telebox/utils/env/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telebox-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 telebox-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 telebox-0.9.2/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 telebox-0.9.2/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 telebox-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 telebox-0.9.2/PKG-INFO
```

### Comparing `telebox-0.9.1/telebox/__init__.py` & `telebox-0.9.2/telebox/__init__.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/context/state_machine.py` & `telebox-0.9.2/telebox/context/state_machine.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/context/telegram_bot.py` & `telebox-0.9.2/telebox/context/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/context/utils.py` & `telebox-0.9.2/telebox/context/utils.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/__init__.py` & `telebox-0.9.2/telebox/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/dispatcher.py` & `telebox-0.9.2/telebox/dispatcher/dispatcher.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/typing.py` & `telebox-0.9.2/telebox/dispatcher/typing.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/enums/event_type.py` & `telebox-0.9.2/telebox/dispatcher/enums/event_type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/__init__.py` & `telebox-0.9.2/telebox/dispatcher/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/error_filter.py` & `telebox-0.9.2/telebox/dispatcher/filters/error_filter.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event_filter.py` & `telebox-0.9.2/telebox/dispatcher/filters/event_filter.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/error/reg_exp_text.py` & `telebox-0.9.2/telebox/dispatcher/filters/error/reg_exp_text.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/error/text.py` & `telebox-0.9.2/telebox/dispatcher/filters/error/text.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/error/type.py` & `telebox-0.9.2/telebox/dispatcher/filters/error/type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/__init__.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/__init__.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/callback_data.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/callback_data.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/cashtag.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/cashtag.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/chat_id.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/chat_id.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/chat_type.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/chat_type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/command.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/command.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/forwarded_message.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/forwarded_message.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/hashtag.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/hashtag.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/media_group_content_type.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/media_group_content_type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/mention.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/mention.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/message_content_type.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/message_content_type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/non_standard_command.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/non_standard_command.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/reg_exp_text.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/reg_exp_text.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/reply_message.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/reply_message.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/sender_contact.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/sender_contact.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/simple_callback_data.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/simple_callback_data.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/state.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/state.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/text.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/text.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/text_mention.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/text_mention.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/filters/event/user_id.py` & `telebox-0.9.2/telebox/dispatcher/filters/event/user_id.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/middlewares/middleware.py` & `telebox-0.9.2/telebox/dispatcher/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/middlewares/middlewares/callback_data.py` & `telebox-0.9.2/telebox/dispatcher/middlewares/middlewares/callback_data.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/event_queue.py` & `telebox-0.9.2/telebox/dispatcher/utils/event_queue.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/events.py` & `telebox-0.9.2/telebox/dispatcher/utils/events.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/media_group.py` & `telebox-0.9.2/telebox/dispatcher/utils/media_group.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/server_root.py` & `telebox-0.9.2/telebox/dispatcher/utils/server_root.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/call_tracker.py` & `telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/call_tracker.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/rate_limit.py` & `telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/rate_limit.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/dispatcher/utils/rate_limiter/rate_limiter.py` & `telebox-0.9.2/telebox/dispatcher/utils/rate_limiter/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/state_machine/errors.py` & `telebox-0.9.2/telebox/state_machine/errors.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/state_machine/machine.py` & `telebox-0.9.2/telebox/state_machine/machine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import Optional, Any
-import contextlib
 
 from telebox.state_machine.state import State
 from telebox.state_machine.storages.storage import AbstractStateStorage
 from telebox.state_machine.manager import StateManager
 from telebox.state_machine.transition_scheme import TransitionScheme
 from telebox.state_machine.magazine import StateMagazine
 from telebox.state_machine.errors import (
     DestinationStateNotFoundError,
     NextStateNotFoundError,
-    PreviousStateNotFoundError,
-    StateExistsError
+    PreviousStateNotFoundError
 )
 from telebox.dispatcher.handlers.event import AbstractEventHandler
 from telebox.dispatcher.typing import Event
 
 
 class StateMachine:
 
@@ -44,17 +42,34 @@
             source_state=source_state,
             destination_state=destination_state,
             handler=handler,
             direction=direction
         )
 
         for i in (source_state, destination_state):
-            with contextlib.suppress(StateExistsError):
+            if not self.check_state(i):
                 self.add_state(i)
 
+    def check_state(self, state: State) -> bool:
+        return self._state_manager.check_state(state)
+
+    def check_transition(
+        self,
+        source_state: State,
+        destination_state: State,
+        handler: AbstractEventHandler,
+        direction: Optional[str] = None
+    ) -> bool:
+        return self._transition_scheme.check_transition(
+            source_state,
+            destination_state,
+            handler,
+            direction
+        )
+
     def get_state(self, *, chat_id: int, user_id: Optional[int] = None) -> State:
         magazine = self._state_manager.load_magazine(chat_id=chat_id, user_id=user_id)
 
         return self._state_manager.get_state(magazine.current_state)
 
     def set_next_state(
         self,
```

### Comparing `telebox-0.9.1/telebox/state_machine/magazine.py` & `telebox-0.9.2/telebox/state_machine/magazine.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/state_machine/manager.py` & `telebox-0.9.2/telebox/state_machine/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,31 @@
         return self._initial_state
 
     @property
     def states(self) -> set[State]:
         return set(self._states.values())
 
     def add_state(self, state: State) -> None:
-        if state.name in self._states:
-            raise StateNameExistsError(
-                "State name {state_name!r} already exists!",
-                state_name=state.name
-            )
-
         if state in self._states.values():
             raise StateExistsError(
                 "State {state!r} already exists!",
                 state=state
             )
 
+        if state.name in self._states:
+            raise StateNameExistsError(
+                "State name {state_name!r} already exists!",
+                state_name=state.name
+            )
+
         self._states[state.name] = state
 
+    def check_state(self, state: State) -> bool:
+        return state in self.states
+
     def get_state(self, name: str) -> State:
         try:
             return self._states[name]
         except KeyError:
             raise StateNotFoundError(
                 "State with name {state_name!r} not found!",
                 state_name=name
```

### Comparing `telebox-0.9.1/telebox/state_machine/transition_scheme.py` & `telebox-0.9.2/telebox/state_machine/transition_scheme.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,26 @@
                 direction=direction
             )
 
         source_states = self._transitions.setdefault(source_state, {})
         handlers = source_states.setdefault(handler, {})
         handlers[direction] = destination_state
 
+    def check_transition(
+        self,
+        source_state: State,
+        destination_state: State,
+        handler: AbstractEventHandler,
+        direction: Optional[str] = None
+    ) -> bool:
+        try:
+            return self._transitions[source_state][handler][direction] is destination_state
+        except KeyError:
+            return False
+
     def get_destination_state(
         self,
         source_state: State,
         handler: AbstractEventHandler,
         direction: Optional[str] = None
     ) -> State:
         try:
```

### Comparing `telebox-0.9.1/telebox/state_machine/storages/storages/file.py` & `telebox-0.9.2/telebox/state_machine/storages/storages/file.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/state_machine/storages/storages/memory.py` & `telebox-0.9.2/telebox/state_machine/storages/storages/memory.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/errors.py` & `telebox-0.9.2/telebox/telegram_bot/errors.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/serializer.py` & `telebox-0.9.2/telebox/telegram_bot/serializer.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/telegram_bot.py` & `telebox-0.9.2/telebox/telegram_bot/telegram_bot.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/utils.py` & `telebox-0.9.2/telebox/telegram_bot/utils.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/consts/country_codes.py` & `telebox-0.9.2/telebox/telegram_bot/consts/country_codes.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/consts/currencies.py` & `telebox-0.9.2/telebox/telegram_bot/consts/currencies.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/consts/language_codes.py` & `telebox-0.9.2/telebox/telegram_bot/consts/language_codes.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/enums/message_content_type.py` & `telebox-0.9.2/telebox/telegram_bot/enums/message_content_type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/enums/update_content_type.py` & `telebox-0.9.2/telebox/telegram_bot/enums/update_content_type.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/__init__.py` & `telebox-0.9.2/telebox/telegram_bot/types/__init__.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/__init__.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/bot_command_scope.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/callback_query.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/callback_query.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_administrator_rights.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_invite_link.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_join_request.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_member.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_member.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_administrator.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_administrator.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_restricted.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_restricted.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_member_updated.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/chat_permissions.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/encrypted_passport_element.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/encrypted_passport_element.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/game.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/game.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_keyboard_button.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_article.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_audio.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_audio.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_document.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_gif.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_gif.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_mpeg4_gif.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_photo.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_sticker.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_video.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_cached_voice.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_contact.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_document.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_gif.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_gif.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_location.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_mpeg4_gif.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_photo.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_venue.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_video.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/inline_query_result_voice.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_invoice_message_content.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_invoice_message_content.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_media.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_media.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_media_animation.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_media_audio.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_media_document.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_media_document.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_media_video.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_media_video.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/input_message_content.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/input_message_content.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/keyboard_button.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/message.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/message.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/passport_element_error.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/passport_element_error.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/poll.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/poll.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/pre_checkout_query.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/sticker.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/sticker.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/update.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/update.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/user.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/user.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/telegram_bot/types/types/webhook_info.py` & `telebox-0.9.2/telebox/telegram_bot/types/types/webhook_info.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/utils/named_set.py` & `telebox-0.9.2/telebox/utils/named_set.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/utils/task_executor.py` & `telebox-0.9.2/telebox/utils/task_executor.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/utils/thread_pool.py` & `telebox-0.9.2/telebox/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/telebox/utils/callback_data_builders/builders/separatory.py` & `telebox-0.9.2/telebox/utils/callback_data_builders/builders/separatory.py`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/LICENSE` & `telebox-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telebox-0.9.1/pyproject.toml` & `telebox-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "telebox"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Abstract-X", email="abstract-x-mail@protonmail.com" },
 ]
 description = "A Python framework for creating Telegram bots."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `telebox-0.9.1/PKG-INFO` & `telebox-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebox
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python framework for creating Telegram bots.
 Project-URL: Homepage, https://github.com/Abstract-X/telebox
 Project-URL: Bug Tracker, https://github.com/Abstract-X/telebox/issues
 Author-email: Abstract-X <abstract-x-mail@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Abstract-X
```

